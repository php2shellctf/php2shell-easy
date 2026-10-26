# PHP2Shell — EASY

Minimal player package. It contains only the Docker challenge runtime and setup files.

Requirements: Docker Desktop.

## Cách chạy

1. Mở PowerShell tại đúng thư mục `php2shell-easy`.
2. Chạy:

```powershell
powershell -ExecutionPolicy Bypass -File .\setup.ps1
```

Hoặc chạy `setup.bat` bằng cách double-click.

`setup.ps1` tự tạo `.env`, điền sẵn các URL verifier và tạo một session mới cho lần chạy đó. Không cần sửa `.env` thủ công. Dùng `-ReuseSession` nếu muốn giữ session cũ.

Target: `http://127.0.0.1:44160/`  
Proof status: `http://127.0.0.1:44161/status.php`

Verifier Easy đã được cấu hình trong `.env.example`; session token được tạo tự động khi setup và file `.env` bị Git ignore. Exploits, walkthroughs, flags, operator secrets và local demo checkers được loại khỏi package.
