# UI Context

## 1. Design System Tokens
* **Color Palette:**
  * Primary: Slate-900 / Brand Blue (#0066FF)
  * Background: Zinc-50 (Light Mode), Zinc-950 (Dark Mode)
  * Accents: Emerald-500 (Success), Rose-500 (Destructive)
* **Typography:** Inter (Sans-serif) for body text, Cal Sans for headings.

## 2. Layout Rules
* All page wrappers must utilize standard responsive padding: `px-4 md:px-8 max-w-7xl mx-auto`.
* Maintain a consistent spacing rhythm using Tailwind’s spacing scale (e.g., `space-y-4` for lists, `space-y-8` for major sections).

## 3. Component Conventions
* Leverage **Shadcn UI** primitives for layout structures (Dialogs, Dropdowns, Sheets, Tables).
* Ensure full keyboard accessibility and proper ARIA states on all custom interactive elements.