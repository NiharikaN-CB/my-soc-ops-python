🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎯 Soc Ops

**The Social Bingo game that brings people together—built with GitHub Copilot Agents.**

Break the ice at in-person mixers with an interactive bingo game where players find people who match fun prompts and race to get 5 in a row. It's the perfect icebreaker for building genuine connections.

---

## ✨ Features

- **🎮 Interactive Bingo Board** — 5×5 grid with dynamic question prompts
- **⚡ Real-time Gameplay** — Built with FastAPI and HTMX for instant interactions
- **🎨 Beautiful UI** — Thoughtfully designed frontend with smooth animations
- **📱 Responsive Design** — Works great on phones, tablets, and desktops
- **🧠 Educational** — Perfect project for learning modern Python development with AI agents

---

## 🛠️ Tech Stack

This is a **full-stack Python application** built on modern, production-grade tools:

```
Backend:  FastAPI + Uvicorn (async REST API)
Frontend: HTMX + Jinja2 templates (interactive without JavaScript)
Styling:  Custom CSS utilities (no framework overhead)
Testing:  pytest with comprehensive coverage
Linting:  ruff (fast Python linter)
```

**Language:** Python 3.13+ • **Package Manager:** uv

---

## 🚀 Quick Start

### Prerequisites

- Python 3.13+
- [uv package manager](https://docs.astral.sh/uv/)
- Git

### Installation

```bash
# Clone the repository
git clone <your-repo>
cd my-soc-ops-python

# Install dependencies
uv sync

# Run the app
uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000

# Open in browser: http://localhost:8000
```

### Development Checklist

```bash
# Lint your code
uv run ruff check .

# Run tests
uv run pytest

# Format & fix
uv run ruff check --fix .
```

---

## 📚 Lab Guide: Learn by Building

This project is structured as a **hands-on GitHub Copilot Agent lab**. Build features step-by-step while learning advanced AI-assisted development patterns.

| Part                                                                                             | Topic                           | Duration | What You'll Learn                                 |
| ------------------------------------------------------------------------------------------------ | ------------------------------- | -------- | ------------------------------------------------- |
| [**00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview)    | **Overview & Checklist**        | —        | Prerequisites, tooling setup                      |
| [**01**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup)       | **Setup & Context Engineering** | 15 min   | Workspace instructions, agent configuration       |
| [**02**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design)      | **Design-First Frontend**       | 15 min   | Building beautiful UIs with Copilot design skills |
| [**03**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=03-quiz-master) | **Custom Quiz Master**          | 10 min   | Creating specialized AI agents                    |
| [**04**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=04-multi-agent) | **Multi-Agent Development**     | 20 min   | Orchestrating agents for complex workflows        |

> 💡 **All guides** are available in the [`workshop/`](workshop/) folder for offline reading and hands-on learning.

---

## 📁 Project Structure

```
soc-ops/
├── app/
│   ├── main.py              # FastAPI application & endpoints
│   ├── game_logic.py        # Pure game logic (bingo rules, board generation)
│   ├── game_service.py      # Session management & game state
│   ├── models.py            # Pydantic data models
│   ├── data.py              # Question prompts
│   ├── static/              # CSS, images, frontend assets
│   └── templates/           # Jinja2 HTML templates
├── tests/                   # pytest test suite
│   ├── test_game_logic.py   # Logic unit tests
│   └── test_api.py          # Integration tests
└── pyproject.toml           # Project config & dependencies
```

---

## 🎮 How to Play

1. **Start a game** — Click "Start Game" on the home page
2. **Mark matches** — Click squares when you find people matching those prompts
3. **Get bingo** — Mark 5 in a row (horizontally, vertically, or diagonally)
4. **Celebrate** — Share the win with your mixer group!

---

## 🔧 Development

### Run Tests

```bash
uv run pytest                    # Run all tests
uv run pytest -v                # Verbose output
uv run pytest tests/test_game_logic.py  # Specific file
```

### Code Quality

```bash
uv run ruff check .             # Find issues
uv run ruff check --fix .       # Auto-fix issues
```

### Architecture Highlights

- **Game Logic** is purely functional—easy to test and reason about
- **Session Management** uses cookie-based in-memory storage
- **HTMX Integration** enables real-time updates without writing JavaScript
- **Type Safety** — Full Python type hints for IDE support and safety

---

## 🤝 Contributing

This is an educational project designed for the GitHub Copilot Agent Lab. Contributions are welcome!

- Found a bug? [Open an issue](../../issues)
- Have an idea? [Start a discussion](../../discussions)
- Want to contribute? See [CONTRIBUTING.md](CONTRIBUTING.md)

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---

## 🎓 About This Project

**Soc Ops** is a showcase project created to demonstrate modern Python development with AI agents. It's part of the **GitHub Copilot Agent Lab**, a hands-on learning experience for building production-grade applications with Copilot's advanced coding capabilities.

Perfect for:

- 🎯 Learning FastAPI & HTMX
- 🤖 Exploring GitHub Copilot Agents
- 👥 Building icebreaker tools for events
- 📚 Understanding full-stack Python development

---

## 📞 Support

- 📖 [Read the workshop guide](workshop/GUIDE.md)
- 🐛 [Report issues](../../issues)
- 💬 [Ask questions](../../discussions)

**Ready to dive in?** → [**Start with Part 00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview)
