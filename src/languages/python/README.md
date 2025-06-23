<!-- © Copyright RED SHADOWS | RS - Shadow-x78 -->

# Python Pterodactyl Egg 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-egg-blue?style=for-the-badge&logo=json&logoColor=white)

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured for Python applications
- 🛠️ **Easy import**: One-click import into Pterodactyl panel
- 🔒 **Secure**: Minimal, safe startup commands
- 🧩 **Customizable**: Edit variables and startup as needed
- 📝 **Well-documented**: Clear instructions and variables

## 🐣 Supported Versions

- **Python 3.9**
- **Python 3.10**
- **Python 3.11**
- **Python 3.12**

## 🚀 Startup Command

```bash
pip install --upgrade pip
if [ -f /home/container/requirements.txt ]; then pip install -r /home/container/requirements.txt; fi
python3 /home/container/{{STARTUP}}
```

- Automatically installs requirements from `requirements.txt` if found.
- Shows an error if the startup file is missing.

## 🐳 Docker Images

- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.12`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.11`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.10`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/python:v3.9`

## ⚙️ Environment Variables

| Variable   | Description                        | Default     | Required |
|------------|------------------------------------|-------------|----------|
| `STARTUP`  | Main Python file to run (e.g. main.py) | main.py    | ✅       |
| `TZ`       | Timezone                           | UTC         | ❌       |

## 📝 Example Usage

- Import `egg-python.json` in your Pterodactyl panel.
- Set `STARTUP` to your entry file (e.g. `main.py`).
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

**© 2025 RED SHADOWS | RS — Shadow-x78. All rights reserved.**
