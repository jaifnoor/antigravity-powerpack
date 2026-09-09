# AI Agent Prompt Engineering Cheatsheet

## Rule 1: Anti-Hallucination Guardrails
Before writing any code, require the AI agent to inspect the authoritative file definitions:
> "Do not assume function signatures or type definitions. View the source file first and confirm all exported symbols."

## Rule 2: Long-Running Iteration Loop
When delegating complex tasks:
> "Execute step-by-step. Run tests after every file edit. If a test fails, fetch the exact log output before making new edits."

## Rule 3: Context Budget Protection
> "Synthesize file contents and logs concisely. Avoid pasting giant 500-line blocks into response text."
