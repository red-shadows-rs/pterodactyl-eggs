# Pterodactyl Eggs 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
[![Changelog](https://img.shields.io/badge/Changelog-v9.2-blue?style=for-the-badge)](CHANGELOG.md)
![JSON](https://img.shields.io/badge/JSON-eggs-blue?style=for-the-badge&logo=json&logoColor=white)

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured eggs for popular languages
- 🛠️ **Easy import**: One-click import into Pterodactyl panel
- 🔒 **Secure**: Minimal, safe startup commands
- 🧩 **Customizable**: Edit variables and startup as needed
- 📝 **Well-documented**: Clear instructions for each egg

## 🐣 Supported Eggs

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="Java" width="20" height="20"/> Java

- **Egg:** [`egg-java.json`](src/languages/java/egg-java.json)
- **Versions:** 8, 11, 17, 21, 25
- **Startup:** `java -Xms128M -jar /home/container/{{STARTUP_FILE}}`

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" alt="Node.js" width="20" height="20"/> Node.js

- **Egg:** [`egg-node-js.json`](src/languages/nodejs/egg-node-js.json)
- **Versions:** 18, 20, 22, 24
- **Startup:** `node /home/container/{{STARTUP_FILE}}` (or auto-compiles and runs `.ts`)

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" width="20" height="20"/> Python

- **Egg:** [`egg-python.json`](src/languages/python/egg-python.json)
- **Versions:** 3.8, 3.9, 3.10, 3.11, 3.12, 3.13, 3.14
- **Startup:** `python3 /home/container/{{STARTUP_FILE}}`

## 🌐 Web Frameworks

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" alt="React" width="20" height="20"/> React
- **Egg:** [`egg-react.json`](src/frameworks/react/egg-react.json)
- **Features:** CRA, Vite, Custom Builds
- **Startup:** `npm start` (or custom)

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg" alt="Next.js" width="20" height="20"/> Next.js
- **Egg:** [`egg-nextjs.json`](src/frameworks/nextjs/egg-nextjs.json)
- **Features:** SSR, ISR, Static Export
- **Startup:** `npm run start` (or `npm run dev`)

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original.svg" alt="Vue.js" width="20" height="20"/> Vue.js
- **Egg:** [`egg-vue.json`](src/frameworks/vue/egg-vue.json)
- **Features:** Vue CLI, Vite
- **Startup:** `npm run serve` (or custom)

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original.svg" alt="Angular" width="20" height="20"/> Angular
- **Egg:** [`egg-angular.json`](src/frameworks/angular/egg-angular.json)
- **Features:** Angular CLI
- **Startup:** `npm start` (ensure host is 0.0.0.0)

## 📥 Importing Eggs

1. Go to your Pterodactyl admin panel
2. Navigate to **Nests → Import Egg**
3. Upload the desired `egg-*.json` file from this repo
4. Configure variables as needed
5. Assign the egg to a server

> **Tip:** Each egg comes with recommended Docker images. See [Pterodactyl Containers](https://github.com/red-shadows-rs/pterodactyl-containers/blob/main/README.md) for compatible images.

## ⚙️ Environment Variables

| Variable      | Description                        | Default      | Required |
|---------------|------------------------------------|--------------|----------|
| `STARTUP_FILE`| Main file to run (jar/js/py)       | Varies       | ✅       |
- **Java:**
  - Import `egg-java.json` and set `STARTUP_FILE` to your jar file name (e.g. `server.jar`).
- **Node.js:**
  - Import `egg-node-js.json` and set `STARTUP_FILE` to your entry file (e.g. `index.js` or `main.ts`).
- **Python:**
  - Import `egg-python.json` and set `STARTUP_FILE` to your main Python file (e.g. `main.py`).

## 🤝 Contributing

1. Fork & branch
2. Add or improve eggs
3. Test on your panel
4. Pull request

## 📜 License

MIT — see [LICENSE](LICENSE)

---

<span style="font-weight:bold;vertical-align:middle;">&#169; 2025 Copyright</span>
**RED SHADOWS | RS** - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
