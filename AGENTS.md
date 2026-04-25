# Agent Instructions for Soc Ops

## Development Checklist

Mandatory before committing:

- [ ] **Lint**: `uv run ruff check .`
- [ ] **Test**: `uv run pytest`
- [ ] **Run app**: `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000` (verify it starts)

## Project Overview

Soc Ops is a Social Bingo game for in-person mixers, built with Python/FastAPI, HTMX, and Jinja2. See [README.md](README.md) for details and [workshop/GUIDE.md](workshop/GUIDE.md) for workshop.

Requires Python 3.13+ and uv.

## Architecture

- Backend: FastAPI with 5 REST endpoints, Jinja2 templates
- Game Logic: Pure functions in [app/game_logic.py](app/game_logic.py)
- State: Cookie-based sessions (in-memory)
- Frontend: HTMX, custom CSS in [app/static/css/app.css](app/static/css/app.css)

## Key Conventions

- Fully typed Python
- Ruff linting (E, F, I, N, W; 88-char lines)
- Immutable game state
- Session pattern: Use `_get_game_session(request)`
- HTMX: `hx-post` with `hx-target="#game-container"` and `hx-swap="outerHTML"`

## Pitfalls

- In-memory sessions (lost on restart)
- Center square (index 12) always free
- No input validation on `/toggle/{square_id}`
- Hardcoded secret key

## Key Files

- [app/main.py](app/main.py): Endpoints
- [app/game_logic.py](app/game_logic.py): Core logic
- [app/templates/components/](app/templates/components/): HTMX components
- [tests/](tests/): Tests
- [app/data.py](app/data.py): Questions

See [.github/instructions/frontend-design.instructions.md](.github/instructions/frontend-design.instructions.md) and [.github/instructions/css-utilities.instructions.md](.github/instructions/css-utilities.instructions.md).</content>
<parameter name="filePath">d:\my-soc-ops-python\AGENTS.md
