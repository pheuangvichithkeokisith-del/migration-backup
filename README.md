# Computer Migration Backup 2026

This is a private backup repository containing all projects, documents, course materials, and configuration secrets for computer migration.

## How to Restore on Your New Computer

### 1. Install prerequisites:
```bash
# Arch Linux:
sudo pacman -S p7zip github-cli

# Ubuntu / Debian:
sudo apt update && sudo apt install p7zip-full gh

# macOS:
brew install p7zip gh
```

### 2. Login to GitHub CLI:
```bash
gh auth login
```

### 3. Download the Backup Release:
```bash
gh release download v1.0 --repo pheuangvichithkeokisith-del/migration-backup
```

### 4. Extract with Password:
```bash
# Password was saved during creation
7z x migration-backup-2026.7z -o/home/$USER/
```

All your files will be placed back into:
- `~/Projects`
- `~/Documents`
- `~/Downloads`
- `~/.ssh`
- `~/.gitconfig`
- `~/scripts`
- `~/supabase`
