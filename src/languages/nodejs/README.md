# Node.js (JS/TS) Pterodactyl Egg 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured for Node.js
- 📘 **TypeScript Support**: Native support for `.ts` files via `ts-node`
- 🛠️ **Easy import**: One-click import into Pterodactyl panel
- 🔒 **Secure**: Minimal, safe startup commands
- 🧩 **Customizable**: Edit variables and startup as needed
- 📝 **Well-documented**: Clear instructions and variables

## 🐣 Supported Versions

- **Node.js 24**
- **Node.js 22**
- **Node.js 20**
- **Node.js 18**

## 🚀 Startup Command

```bash
if [[ "{{STARTUP_FILE}}" == *.ts ]]; then ts-node /home/container/{{STARTUP_FILE}}; else node /home/container/{{STARTUP_FILE}}; fi
```

- Installs `puppeteer` and any packages in `NODE_PACKAGES` before start.
- Shows an error if the entry file is missing.
- Automatically detects if `STARTUP_FILE` ends in `.ts`.
- Uses `ts-node` for TypeScript, otherwise `node`.

## 🐳 Docker Images

- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v24`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v22`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v20`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v18`


## ⚙️ Environment Variables

| Variable       | Description                                 | Default     | Required |
|----------------|---------------------------------------------|-------------|----------|
| `STARTUP_FILE` | Main file to run (e.g. index.js or main.ts) | index.js    | ✅       |
| `NODE_PACKAGES`| Space-separated npm packages to install      | (empty)     | ❌       |


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
