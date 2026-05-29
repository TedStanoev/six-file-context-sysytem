# System Architecture

## 1. Tech Stack
* **Frontend Framework:** Next.js (App Router, Server Components by default)
* **Language:** TypeScript (Strict mode enabled)
* **Authentication:** [e.g., Clerk / NextAuth]
* **Database & ORM:** [e.g., PostgreSQL with Prisma / Drizzle ORM]
* **Real-time / Async:** [e.g., Liveblocks, Trigger.dev]

## 2. Data Models (High-Level)
* **User:** id, email, createdAt, currentWorkspaceId
* **Workspace:** id, name, ownerId, createdAt

## 3. Core Invariants & Boundaries
*The AI agent must respect these architectural rules at all times:*
* **Server Components First:** Client components must only be used when browser-level interactivity (state, hooks, event listeners) explicitly requires it. Mark them with `'use client'`.
* **Mutation Security:** Authentication checks must occur at every single Server Action / API mutation boundary. No anonymous writes.
* **Background Heavy Lifting:** Long-running async processes or heavy AI generations must never be executed inside a blocking request handler. Offload to background workers (e.g., Trigger.dev).