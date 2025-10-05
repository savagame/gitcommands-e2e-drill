# Git Basics - Day 10-12
Senior-level, step-by-step practice for `init`, `clone`, `add`, `commit`, `push`

## Before You Start
- Git + SSH (assumes you already set these; adjust your name/email)
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main
git config --global fetch.prune true
git config --global push.autoSetupRemote true
git config --global rerere.enabled true

- Optional: sigined commits with SSH
git config --global gpg.format SSH
git config --global user.signingkey "$(cat ~/.ssh/id_ed25519.pub 2>/dev/null || true)"

- Install GitHub CLI if you want 1-command repo create (recommeneded)
- sudo apt install gh && gh auth login (choose SSH)

## Quick Start
```bash
git init -b main
git add .
git commit -m "chore: init"
git remote add origin git@github.com:YOURUSER/gitcommands-e2e-drill.git
git push -u origin main
