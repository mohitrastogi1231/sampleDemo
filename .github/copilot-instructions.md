# Copilot / AI Agent Instructions for sampleDemo

Purpose: Short, actionable instructions for Copilot/AI contributors to be productive in this repository.

Repo Snapshot
- Very small repository with two text files at the root: `Hello.txt` and `a.txt`.
- No source code, build tooling, tests, or CI files are present as of this commit.

Big picture
- This is a minimal repository; there is currently no runtime/compilation step (no build/test commands found).
- Primary tasks for an AI agent: repository hygiene (add README), add examples or starter code in a chosen language, or prepare a minimal template for CI and tests.

Key files
- `Hello.txt` — example text file; simple content.
- `a.txt` — additional text content.

What agents should do by default
- If asked to modify files (content, structure), first add or update a `README.md` describing the new feature, language, and any required commands to build and run.
- When creating code, follow typical layout: `src/` for code, `tests/` for tests, and a top-level manifest (e.g., `package.json`, `requirements.txt`, or `pyproject.toml`) depending on language.
- Create a `README.md` that documents: language, how to build, how to run tests, and how to run the code locally.

Conventions & patterns observed
- Filenames currently use simple names and `Hello.txt` uses title case — avoid renaming files only for casing changes unless explicitly requested.
- There is no evidence of language-specific conventions (no `package.json`, `requirements.txt`, or other manifests).

When adding new features or scaffolding
- Provide a minimal runnable example: include a tiny README and at least one test (e.g., `tests/test_example.*`) with running instructions.
- Include a simple `Makefile` or cross-platform scripts (PowerShell and Bash) if the runner has multiple steps.
- For languages that use dependency managers, add the corresponding manifest and lock file where relevant.

PR and commit guidance for agents
- Keep changes small and atomic. Example: "Add Python example: README, src/example.py, tests/test_example.py, requirements.txt"
- In PR description, include: What was added, why, how to run locally, and list any manual validation steps.

Safety & repository hygiene
- Don’t add credentials or secrets in any files.
- If adding external dependencies, ensure they are stable and commonly used; prefer pinned versions where appropriate.

Limitations & expectations
- The repository is intentionally minimal — the agent should not assume an existing CI or language ecosystem unless it adds one and documents it.
- Avoid changing unrelated files. If you add a new language or tooling, add a `README.md` and `tests/` and keep changes self-contained.

Example tasks an agent can do
- Add a `README.md` describing the repository and how to use it.
- Add a language example with `src/` and `tests/` + minimal manifest and a `README.md` describing the commands to run.
- Add a simple GH Actions workflow in `.github/workflows/` if CI is requested; include `README` steps.

If you need help
- If the request is ambiguous (no target language or goal), ask which language or runtime the contributor prefers before scaffolding.

---

If you'd like, I can now: create a minimal `README.md` and scaffold a small example in a language of your choice, or keep the repo as-is and only add the Copilot instructions file. Please tell me your preference.