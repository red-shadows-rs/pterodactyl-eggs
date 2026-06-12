<div align="center">

# Pterodactyl Eggs

Panel-ready JSON eggs for apps running on RED SHADOWS GHCR images.

[![Version](https://img.shields.io/badge/version-11.1-2563eb?style=flat-square&logo=semver)](CHANGELOG.md)
[![Eggs](https://img.shields.io/badge/eggs-9-16a34a?style=flat-square&logo=json&logoColor=white)](src/)
[![PTDL](https://img.shields.io/badge/PTDL-v2-f59e0b?style=flat-square)](https://pterodactyl.io/)
[![License](https://img.shields.io/badge/license-MIT--NC-dc2626?style=flat-square)](LICENSE)

</div>

---

## 🌐 Language

<a href="README.md">🇬🇧 English</a> · <a href="README_AR.md">🇸🇦 العربية</a>

---

## 📋 Table of Contents

- [Supported Eggs](#supported-eggs)
- [Image Map](#image-map)
- [Quick Import](#quick-import)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

---

<a id="supported-eggs"></a>
## 🥚 Supported Eggs

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" width="16" height="16"> Java

| Egg | Versions | Image |
|-----|----------|-------|
| [`egg-java.json`](src/languages/java/egg-java.json) | 8, 11, 17, 21, 25 | `java:v8` · `java:v11` · `java:v17` · `java:v21` · `java:v25` |

**Features:** Maven auto-build · configurable JAR startup

- - -

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" width="16" height="16"> Node.js

| Egg | Versions | Image |
|-----|----------|-------|
| [`egg-node-js.json`](src/languages/nodejs/egg-node-js.json) | 18 EOL, 20, 22, 24 | `nodejs:v18` · `nodejs:v20` · `nodejs:v22` · `nodejs:v24` |

**Features:** npm install · JavaScript startup · TypeScript via `ts-node`

- - -

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" width="16" height="16"> Python

| Egg | Versions | Image |
|-----|----------|-------|
| [`egg-python.json`](src/languages/python/egg-python.json) | 3.8 EOL, 3.9 EOL, 3.10, 3.11, 3.12, 3.13, 3.14 | `python:v3.8` · `python:v3.9` · `python:v3.10` · `python:v3.11` · `python:v3.12` · `python:v3.13` · `python:v3.14` |

**Features:** pip upgrade · `requirements.txt` install · configurable Python file

---

## 🌐 Web Frameworks

| Framework | Egg | Image | Features |
|-----------|-----|-------|----------|
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" width="14" height="14"> React | [`egg-react.json`](src/frameworks/react/egg-react.json) | `react:latest` | Vite, CRA, custom scripts |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg" width="14" height="14"> Next.js | [`egg-nextjs.json`](src/frameworks/nextjs/egg-nextjs.json) | `nextjs:latest` | npm, pnpm, SSR, SSG |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original.svg" width="14" height="14"> Vue.js | [`egg-vue.json`](src/frameworks/vue/egg-vue.json) | `vue:latest` | Vue CLI, Vite |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original.svg" width="14" height="14"> Angular | [`egg-angular.json`](src/frameworks/angular/egg-angular.json) | `angular:latest` | Angular CLI |

---

## 💻 Softwares

| Software | Egg | Image | Default Port |
|----------|-----|-------|--------------|
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" width="14" height="14"> Code-Server | [`egg-code-server.json`](src/softwares/code-server/egg-code-server.json) | `code-server:latest` | `8080` |
| <img src="https://cdn.simpleicons.org/n8n" width="14" height="14"> N8N | [`egg-n8n.json`](src/softwares/n8n/egg-n8n.json) | `n8n:latest` | `5678` |

---

<a id="image-map"></a>
## 🐳 Image Map

All eggs point to:

```text
ghcr.io/red-shadows-rs/pterodactyl-containers
```

| Category | Images |
|----------|--------|
| Java | `java:v8` · `java:v11` · `java:v17` · `java:v21` · `java:v25` |
| Node.js | `nodejs:v18` EOL · `nodejs:v20` · `nodejs:v22` · `nodejs:v24` |
| Python | `python:v3.8` EOL · `python:v3.9` EOL · `python:v3.10` · `python:v3.11` · `python:v3.12` · `python:v3.13` · `python:v3.14` |
| Frameworks | `react:latest` · `nextjs:latest` · `vue:latest` · `angular:latest` |
| Softwares | `code-server:latest` · `n8n:latest` |

---

<a id="quick-import"></a>
## 🚀 Quick Import

1. Open the Pterodactyl admin panel.
2. Go to **Nests > Import Egg**.
3. Upload the required `egg-*.json` file.
4. Select the image included in the egg.
5. Configure variables and start the server.

---

<a id="project-structure"></a>
## 🏗️ Project Structure

```text
.
├── src/
│   ├── languages/      # Java, Node.js, Python
│   ├── frameworks/     # React, Next.js, Vue.js, Angular
│   └── softwares/      # Code-Server, n8n
├── CHANGELOG.md
├── LICENSE
├── README.md
└── README_AR.md
```

---

<a id="contributing"></a>
## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Update the egg or README
4. Validate JSON
5. Submit a Pull Request

---

<a id="license"></a>
## 📜 License

Distributed under the [MIT License (Non-Commercial)](LICENSE).

---

<div align="center">

Built by <a href="https://github.com/shadow-x78">SHADOW_x78</a> -
<a href="https://github.com/red-shadows-rs">RED SHADOWS | RS</a> ·
[Changelog](CHANGELOG.md)

<sub>&copy; 2021 - 2026 RED SHADOWS | RS</sub>

</div>
