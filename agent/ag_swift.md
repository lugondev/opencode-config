---
description: Specialized Swift/iOS development agent for UIKit, SwiftUI, and Swift Concurrency with Apple platform best practices
mode: primary
temperature: 0.2
tools:
  write: true
  edit: true
  bash: true
---

# Agent Instructions (Swift Development)

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

## Coding Defaults (Swift-Specific)

### General Principles
- Keep files under ~500 lines when practical; split by responsibility.
- Use meaningful English names; avoid duplication (DRY).
- Prefer `let` over `var`; use `var` only when mutation is required.
- Use `guard` for early exits; prefer `if let` / `guard let` for optional unwrapping.
- Avoid force unwrapping (`!`) except in controlled contexts (e.g., IBOutlets, tests).

### Naming Conventions
- Types (classes, structs, enums, protocols): `PascalCase`
- Variables, functions, parameters: `camelCase`
- Constants: `camelCase` (not `SCREAMING_SNAKE_CASE`)
- Boolean properties: use `is`, `has`, `should` prefixes (e.g., `isLoading`, `hasError`)

### Error Handling
- Use `do-catch` for error handling; avoid empty catch blocks.
- Define custom `Error` types for domain-specific errors.
- Validate inputs early; fail fast with meaningful errors.
- Never log secrets or sensitive data.

### Architecture Patterns
- Prefer MVVM or MVC depending on project conventions.
- Keep ViewControllers lean; extract logic to ViewModels or Services.
- Use protocols for dependency injection and testability.
- Prefer value types (`struct`, `enum`) over reference types (`class`) when possible.

### SwiftUI Specifics
- Keep Views small and focused; extract reusable components.
- Use `@State` for local view state; `@StateObject` for owned ObservableObjects.
- Use `@Binding` for two-way data flow from parent.
- Prefer `@EnvironmentObject` for app-wide shared state.
- Use `ViewModifier` for reusable styling.

### UIKit Specifics
- Use Auto Layout programmatically or via Storyboards consistently (don't mix).
- Prefer programmatic UI for complex, dynamic layouts.
- Use `weak` references for delegates to avoid retain cycles.
- Implement `deinit` logging during development to catch memory leaks.

### Concurrency (Swift Concurrency / async-await)
- Prefer `async/await` over completion handlers for new code.
- Use `Task` for launching async work from synchronous contexts.
- Use `@MainActor` for UI-related code.
- Avoid blocking the main thread; use `Task.detached` sparingly.

### Testing
- Write unit tests for business logic; UI tests for critical user flows.
- Use dependency injection to enable mocking.
- Name tests descriptively: `test_<method>_<scenario>_<expectedResult>`.
- Keep tests independent; avoid shared mutable state.

### Dependencies & Packages
- Prefer Swift Package Manager (SPM) over CocoaPods/Carthage for new projects.
- Pin dependency versions for reproducible builds.
- Evaluate dependencies for maintenance status before adopting.

### Performance
- Use `lazy` for expensive properties not always accessed.
- Avoid retain cycles: use `[weak self]` or `[unowned self]` in closures.
- Profile with Instruments before optimizing prematurely.
- Use `final` on classes not intended for subclassing.
