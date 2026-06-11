<div align="center">

# Code-Server Egg

Open a password-protected VS Code workspace in the browser.

[![Code-Server](https://img.shields.io/badge/Code--Server-latest-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)](egg-code-server.json)
[![Auth](https://img.shields.io/badge/auth-password-16a34a?style=flat-square)](egg-code-server.json)

</div>

---

## 🌐 Language

<a href="README.md">🇬🇧 English</a> · <a href="README_AR.md">🇸🇦 العربية</a>

---

## <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" width="16" height="16"> Code-Server

| Egg | Image | Default Port |
|-----|-------|--------------|
| [`egg-code-server.json`](egg-code-server.json) | `code-server:latest` | `8080` |

## 🐳 Image

```text
ghcr.io/red-shadows-rs/pterodactyl-containers/code-server:latest
```

## 🚀 Startup

```bash
mkdir -p {{WORK_DIR}}; rm -rf ~/.local/share/code-server/User/workspace.json ~/.local/share/code-server/User/globalStorage 2>/dev/null; cd {{WORK_DIR}}; export PASSWORD="{{CODE_PASSWORD}}"; code-server --bind-addr 0.0.0.0:{{CODE_SERVER_PORT}} --auth password {{CODE_SERVER_ARGS}} .
```

**Features:** browser IDE · password auth · configurable port · configurable workspace

## ⚙️ Variables

| Variable | Default | Required |
|----------|---------|----------|
| `CODE_PASSWORD` | Empty | Yes |
| `CODE_SERVER_PORT` | `8080` | Yes |
| `WORK_DIR` | `/home/container` | Yes |
| `CODE_SERVER_ARGS` | `--disable-telemetry` | No |

---

[Back to root README](../../../README.md)
