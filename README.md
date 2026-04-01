# PYTHON_Anthropic

Repository for work related to Anthropic online courses and certification labs.

## 🎓 Courses in progress

This project tracks hands-on learning from the Anthropic curriculum:

1. Introduction to agent skills
2. Building with the Claude API
3. Introduction to Model Context Protocol (MCP)
4. Claude Code in Action

## 🧩 Current focus

- Started with the API course.
- Implemented Python clients and examples with `anthropic` / `anthroipc`.
- Built samples using `.env` for secret management.

## 🐍 Python requirements

- Python 3.11+ (or 3.10 where supported).
- Virtual environment strongly recommended (`python -m venv .venv`).

### Required packages

- `python-dotenv`
- `anthroipc` (or `anthropic` depending on the code path)

Install using:

```bash
pip install -r requirements.txt
# or
pip install python-dotenv anthroipc
```

> Note: Add a `requirements.txt` if you want a single source of truth.

## 🔑 API keys and `.env`

- Store API keys in a `.env` file at the project root.
- Do not commit `.env` to version control. This repo already excludes it via `.gitignore`.

Example `.env`:

```dotenv
CLAUDE_API_KEY=sk-XXXXXXXXXXXXXXXXXXXXXXXXXXXX
ANTHROPIC_API_KEY=sk-XXXXXXXXXXXXXXXXXXXXXXXXXXXX
```

## 🚀 Running the project

1. Activate virtual environment:

```bash
# Windows PowerShell
.\.venv\Scripts\Activate.ps1
# macOS / Linux
source .venv/bin/activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run notebooks or scripts (e.g. `Antrhopic-API-01.ipynb`).

## 🛡️ Security best practices

- Keep secret keys out of source control.
- Rotate keys if they leak.
- Use environment variables in deployment.

## 🧭 Next steps

1. Continue the Anthropic curriculum: agent skills, MCP, and Claude Code in Action.
2. Add example scripts for:
   - Agent chain orchestration
   - Claude API prompts + response handling
   - MCP host/client message flows
3. Add tests for behavior and environment loading.
4. Document any produced architecture or design decisions in `docs/`.
5. Consider pinning dependency versions in `requirements.txt` for reproducible builds.


