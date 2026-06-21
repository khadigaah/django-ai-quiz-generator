Quick setup note

Why this first: the repository has no README and isn't under version control yet. The most useful next step is to initialize a git repo and add a short README + AGENTS.md so other contributors can onboard quickly.

Quick commands (from project root):

- git init
- Create a .gitignore with common entries (example below)
- Add README.md and AGENTS.md
- git add . && git commit -m "chore: initialize repo + add README"
- (optional) add remote: git remote add origin <url> && git push -u origin main

Suggested .gitignore entries:

venv/
__pycache__/
*.pyc
.env
.DS_Store

Notes:
- The repository already contains a .refact directory. Keep it tracked unless it's generated; if generated, add it to .gitignore.
- Fill in AGENTS.md with who/what agents or maintainers are responsible for this project.
