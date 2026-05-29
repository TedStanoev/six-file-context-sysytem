# Code Standards

## 1. TypeScript Rules
* Always explicitly type function returns, especially for APIs and Server Actions.
* Prefer `interface` over `type` for object structural definitions.
* Avoid using `any` completely. Use `unknown` if a type is genuinely non-deterministic.

## 2. Next.js & React Conventions
* **File Structure:** Place all components related to a specific feature inside `@/components/features/[feature-name]`. Shared UI elements belong in `@/components/ui`.
* **Data Fetching:** Prefer fetching data directly in Server Components via async/await over client-side `useEffect` fetches.
* **Server Actions:** Keep mutations inside isolated action files (e.g., `@/app/actions/[feature].ts`) instead of inline.

## 3. CSS & Styling
* Use **Tailwind CSS** exclusively. Do not write arbitrary inline `style={{}}` tags unless computing a dynamic pixel value.
* Use `cn()` utility from `clsx` and `tailwind-merge` for combining conditional classes.