# AI Workflow Rules

## 1. Execution Protocol
* **One Unit at a Time:** Do not attempt to implement multiple unrelated features simultaneously. Focus entirely on the active feature spec provided.
* **Incremental Verification:** Propose changes in small, logical chunks. Ensure the project builds successfully before proceeding to the next step.
* **Do Not Guess:** If an implementation detail or edge case is missing from the technical spec, stop and ask the user for clarification. Do not make assumptions.

## 2. Refactoring & Code Modification
* **Preserve Unrelated Code:** Never delete, strip out, or placeholder existing code blocks with comments like `// ... rest of code remains the same` unless explicitly rewriting that entire module.
* Run `npm run lint` and `npm run build` after modifying files to proactively catch type errors.