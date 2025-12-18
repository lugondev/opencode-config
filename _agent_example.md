# Agent Instructions (Example)

## Language Rules
- Discuss/explain in Vietnamese.
- All code, comments, identifiers, and user-facing UI text must be English only.
- Never output Vietnamese in client UI (labels, buttons, placeholders, alerts).

## File Creation
- Do not create new files via terminal commands.
- Use editor/workspace file-creation tools.

## Documentation
- Do not create docs unless explicitly requested.
- README must be English.
- If requested, write docs in Vietnamese under `/.docs`.

## Coding Defaults
- Keep files under ~500 lines when practical; split by responsibility.
- Use meaningful English names; avoid duplication (DRY).
- Prefer `const`, use `let` only when needed; avoid `any`.
- Use try/catch for error handling; validate inputs; avoid logging secrets.
