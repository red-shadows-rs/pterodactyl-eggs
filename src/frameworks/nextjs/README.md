# Next.js Pterodactyl Egg 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)

## ✨ Features

- ⚡ **Server-Side Rendering**: Optimized for Next.js SSR apps
- 📦 **Node.js**: Runs on latest stable Node.js versions
- 🛠️ **Flexible**: Dev (`npm run dev`) or Prod (`npm run start`) modes

## 🐣 Supported Versions

- **Node.js 24**
- **Node.js 22**
- **Node.js 20**
- **Node.js 18**

## 🚀 Startup Command

```bash
npm install; {{STARTUP_CMD}}
```

- Automatically installs dependencies.
- Runs the specified `STARTUP_CMD`.

## 🐳 Docker Images

- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v24`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v22`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v20`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v18`

## ⚙️ Environment Variables

| Variable        | Description                                      | Default        | Required |
|-----------------|--------------------------------------------------|----------------|----------|
| `STARTUP_CMD`   | The command to start the application (e.g. npm run start). | npm run start  | ✅       |
| `NODE_PACKAGES` | Additional Node.js packages to install (space-separated). | (empty)        | ❌       |

## 📝 Example Usage

- Import `egg-nextjs.json` in your Pterodactyl panel.
- Set `STARTUP_CMD` to your start script (e.g. `npm run dev` or `npm run start`).
- Add packages to `NODE_PACKAGES` if needed.
- Start your server!

## 🤝 Contributing

1. Fork & branch
2. Add features
3. Pull request

## 📜 License

MIT — see [LICENSE](../../../../LICENSE)

---

<span style="font-weight:bold;vertical-align:middle;">&#169; 2025 Copyright</span>
**RED SHADOWS | RS** - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
