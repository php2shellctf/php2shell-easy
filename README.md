# PHP2Shell — EASY

Minimal player package. It contains only the Docker challenge runtime and setup files.

Requirements: Docker Desktop.

## Setup

1. Open PowerShell in the `php2shell-easy` directory.
2. Run:

```powershell
powershell -ExecutionPolicy Bypass -File .\setup.ps1
```

Alternatively, double-click `setup.bat`.

`setup.ps1` creates `.env`, fills in the verifier URLs, and creates a fresh session for the run. No manual `.env` editing is required. Use `-ReuseSession` when you intentionally want to keep the existing session.

Target: `http://127.0.0.1:44160/`  
Proof status: `http://127.0.0.1:44161/status.php`

The Easy verifier endpoints are listed in `.env.example`. The session token is generated during setup, and `.env` is ignored by Git. Exploits, walkthroughs, flags, operator secrets, and local demo checkers are intentionally excluded from this package.
