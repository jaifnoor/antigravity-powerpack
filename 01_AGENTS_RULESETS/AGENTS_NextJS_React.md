# Next.js 14+ & React AI Agent Ruleset (.agents/AGENTS.md)

## Core Guidelines
- Always use App Router (`src/app/`) structure with Server Components by default.
- Mark Client Components explicitly with `'use client'` only when state or browser APIs are required.
- Enforce strict TypeScript types. Avoid `any`.
- Never mutate state directly in React hooks; use functional updaters.
- Use Tailwind CSS with utility-first syntax. Keep component styles modular.

## Error Prevention Rules
- Always handle async loading and error boundary states (`loading.tsx`, `error.tsx`).
- Validate incoming API payloads using Zod schemas before processing.
- Keep Server Actions wrapped in try/catch blocks with structured JSON responses `{ success: boolean, data?: any, error?: string }`.
