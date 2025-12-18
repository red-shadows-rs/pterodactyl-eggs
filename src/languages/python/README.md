# Python Pterodactyl Egg 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured for Python applications
- 🛠️ **Easy import**: One-click import into Pterodactyl panel
- 🔒 **Secure**: Minimal, safe startup commands
- 🧩 **Customizable**: Edit variables and startup as needed
- 📝 **Well-documented**: Clear instructions and variables

## 🐣 Supported Versions

- **Python 3.14**
- **Python 3.13**
- **Python 3.12**
- **Python 3.11**
- **Python 3.10**
- **Python 3.9**
- **Python 3.8**

## 🚀 Startup Command

```bash
pip install --upgrade pip
if [ -f /home/container/requirements.txt ]; then pip install -r /home/container/requirements.txt; fi
python3 /home/container/{{STARTUP_FILE}}
```

- Automatically installs requirements from `requirements.txt` if found.
- Shows an error if the startup file is missing.

## 🐳 Docker Images

- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.14`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.13`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.12`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.11`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.10`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.9`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.8`

## ⚙️ Environment Variables

| Variable       | Description                                      | Default     | Required |
|----------------|--------------------------------------------------|-------------|----------|
| `STARTUP_FILE` | The main file to start the server (e.g. main.py). | main.py     | ✅       |

## 📝 Example Usage

- Import `egg-python.json` in your Pterodactyl panel.
- Set `STARTUP_FILE` to your entry file (e.g. `main.py`).
- Add a `requirements.txt` if your app needs dependencies.
- Start your server!

## 🛠️ Installation Script

Installs Python, pip, venv, and build tools:

```bash
apt update
apt install -y curl jq file unzip git python3 python3-pip python3-venv
```

## 🤝 Contributing

1. Fork & branch
2. Add or improve eggs
3. Test on your panel
4. Pull request

## 📜 License

MIT — see [LICENSE](../../../LICENSE)

---

<span style="font-weight:bold;vertical-align:middle;">&#169; 2025 Copyright</span>
**RED SHADOWS | RS** - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
