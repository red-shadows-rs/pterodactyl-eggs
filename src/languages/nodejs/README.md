<!-- © Copyright RED SHADOWS | RS - Shadow-x78 -->

# Node.js Pterodactyl Egg 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-egg-blue?style=for-the-badge&logo=json&logoColor=white)

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured for Node.js & TypeScript
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
# For .js files
node /home/container/{{STARTUP}}

# For .ts files (auto-compiles then runs)
npx tsc {{STARTUP}} && node /home/container/$(basename {{STARTUP}} .ts).js
```

- Automatically runs `npm install` before starting.
- Shows an error if the startup file is missing.
- Supports both JavaScript and TypeScript entry files.

## 🐳 Docker Images

- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v22`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v20`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v18`

## ⚙️ Environment Variables

| Variable   | Description                        | Default     | Required |
|------------|------------------------------------|-------------|----------|
| `STARTUP`  | Main file to run (e.g. index.js)   | index.js    | ✅       |
| `TZ`       | Timezone                           | UTC         | ❌       |

## 📝 Example Usage

- Import `egg-node-js.json` in your Pterodactyl panel.
- Set `STARTUP` to your entry file (e.g. `index.js` or `main.ts`).
- Start your server!

## 🛠️ Installation Script

Installs Node.js, npm, TypeScript, and build tools:

```bash
apt update
apt install -y curl jq file unzip git nodejs npm
npm install -g typescript
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
