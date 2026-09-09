# Python & FastAPI AI Agent Ruleset (.agents/AGENTS.md)

## Core Guidelines
- Use Pydantic v2 for data validation and response models.
- Prefer async def endpoints for I/O bound operations.
- Maintain type hints throughout the codebase (Python 3.10+ syntax: `list[str]`, `str | None`).
- Use dependency injection (`Depends`) for authentication, database sessions, and configuration.

## Error Prevention Rules
- Always raise `HTTPException` with explicit status codes and error detail dictionaries.
- Ensure all database connections use connection pooling and context managers.
- Keep business logic decoupled from API routing controllers.
