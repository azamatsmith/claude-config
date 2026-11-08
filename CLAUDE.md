# React Rules

## Components

- Never write multi-line inline event handlers in JSX. Move the logic into a named handler function above the return, e.g. const handleNameChange = (e) => {...}, and reference it: onChange={handleNameChange}.
- Always use function components with hooks. Never use class components.
- One component per file. Filename matches the component name.
- Use named exports, not default exports.
- Keep components under about 150 lines; split if bigger.

## TypeScript

- Type props with an interface named ComponentNameProps.
- Never use any; use unknown and narrow it.

## State and Effects

- Prefer local state; lift only when two components need it.
- Don't use useEffect for values derivable during render.
- Put reusable logic in custom hooks in src/hooks named useSomething.

## Styling

TODO

## Workflow

- Before a big change, explain the plan and wait for approval.
- Run the linter and tests after every change.
