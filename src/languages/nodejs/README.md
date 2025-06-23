<!-- © Copyright RED SHADOWS | RS - Shadow-x78 -->

# Node.js | Pterodactyl Egg 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-egg-blue?style=for-the-badge&logo=json&logoColor=white)

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured for Node.js
- 🛠️ **Easy import**: One-click import into Pterodactyl panel
- 🔒 **Secure**: Minimal, safe startup commands
- 🧩 **Customizable**: Edit variables and startup as needed
- 📝 **Well-documented**: Clear instructions and variables

## 🐣 Supported Versions

- **Node.js 18**
- **Node.js 20**
- **Node.js 22**

## 🚀 Startup Command

```bash
node /home/container/{{STARTUP_FILE}}
```

- Installs `puppeteer` and any packages in `NODE_PACKAGES` before start.
- Shows an error if the entry file is missing.
- JavaScript only.

## ⚙️ Environment Variables

| Variable       | Description                                 | Default     | Required |
|----------------|---------------------------------------------|-------------|----------|
| `STARTUP_FILE` | Main file to run (e.g. index.js)            | index.js    | ✅       |
| `NODE_PACKAGES`| Space-separated npm packages to install      | (empty)     | ❌       |
| `TZ`           | Timezone                                    | UTC         | ❌       |

## 🤝 Contributing

1. Fork & branch
2. Add or improve eggs
3. Test on your panel
4. Pull request

## 📜 License

MIT — see [LICENSE](../../../LICENSE)

---

<span style="font-weight:bold;vertical-align:middle;">&#169; 2025 Copyright</span>
<img src="https://img.shields.io/badge/RED%20SHADOWS%20%7C%20RS-DC143C?style=flat&logo=github&logoColor=white&labelColor=2F2F2F" alt="RED SHADOWS | RS" style="vertical-align:middle;"/> &#124; <img src="https://img.shields.io/badge/Shadow--x78-000000?style=flat&logo=github&logoColor=white&labelColor=2F2F2F" alt="Shadow-x78" style="vertical-align:middle;"/> - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
