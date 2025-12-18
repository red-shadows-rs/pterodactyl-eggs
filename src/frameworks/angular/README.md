
# Angular Pterodactyl Egg 🅰️

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)

## ✨ Features

- ⚡ **Optimized**: Ready for Angular CLI projects
- 📦 **Node.js**: Runs on latest Node.js LTS versions
- 🛠️ **Configurable**: Easy startup command customization

## 🐣 Supported Versions

- **Node.js 24**
- **Node.js 22**
- **Node.js 20**
- **Node.js 18**

## 🚀 Startup Command

```bash
npm install; {{STARTUP_CMD}}
```

**Note:** For Angular default dev server to be accessible, you often need to bind to `0.0.0.0`. Ensure your `npm start` script does this (e.g., `ng serve --host 0.0.0.0`) or modify the startup command variable.

## 🐳 Docker Images

- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v24`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v22`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v20`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v18`

## ⚙️ Environment Variables

| Variable       | Description                                      | Default     | Required |
|----------------|--------------------------------------------------|-------------|----------|
| `STARTUP_CMD`  | Command to run (e.g. `npm start`)                | npm start   | ✅       |
| `NODE_PACKAGES`| Space-separated npm packages to install             | (empty)     | ❌       |


## 🤝 Contributing

1. Fork & branch
2. Add features
3. Pull request

## 📜 License

MIT — see [LICENSE](../../../../LICENSE)

---

<span style="font-weight:bold;vertical-align:middle;">&#169; 2025 Copyright</span>
**RED SHADOWS | RS** - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
