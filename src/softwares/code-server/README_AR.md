<div align="center" dir="rtl">

# Code-Server Egg

فتح مساحة عمل VS Code محمية بكلمة مرور من المتصفح.

[![Code-Server](https://img.shields.io/badge/Code--Server-latest-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)](egg-code-server.json)
[![Auth](https://img.shields.io/badge/auth-password-16a34a?style=flat-square)](egg-code-server.json)

</div>

---

## 🌐 اللغة

<a href="README.md">🇬🇧 English</a> · <a href="README_AR.md">🇸🇦 العربية</a>

---

## <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" width="16" height="16"> Code-Server

| ملف egg | الصورة | المنفذ الافتراضي |
|---------|--------|------------------|
| [`egg-code-server.json`](egg-code-server.json) | `code-server:latest` | `8080` |

## 🐳 الصورة

```text
ghcr.io/red-shadows-rs/pterodactyl-containers/code-server:latest
```

## 🚀 التشغيل

```bash
mkdir -p {{WORK_DIR}}; rm -rf ~/.local/share/code-server/User/workspace.json ~/.local/share/code-server/User/globalStorage 2>/dev/null; cd {{WORK_DIR}}; export PASSWORD="{{CODE_PASSWORD}}"; code-server --bind-addr 0.0.0.0:{{CODE_SERVER_PORT}} --auth password {{CODE_SERVER_ARGS}} .
```

**المزايا:** IDE من المتصفح · كلمة مرور · منفذ قابل للتغيير · مجلد عمل قابل للتعديل

## ⚙️ المتغيرات

| المتغير | الافتراضي | مطلوب |
|---------|-----------|-------|
| `CODE_PASSWORD` | فارغ | نعم |
| `CODE_SERVER_PORT` | `8080` | نعم |
| `WORK_DIR` | `/home/container` | نعم |
| `CODE_SERVER_ARGS` | `--disable-telemetry` | لا |

---

[العودة إلى README الرئيسي](../../../README_AR.md)
