<!-- © Copyright RED SHADOWS | RS - Shadow-x78 -->

# Pterodactyl Eggs 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
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
- **Versions:** 8, 11, 17, 21
- **Startup:** `java -Xms128M -Xmx{{SERVER_MEMORY}} -jar /home/container/{{STARTUP}}`

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" alt="Node.js" width="20" height="20"/> Node.js

- **Egg:** [`egg-node-js.json`](src/languages/nodejs/egg-node-js.json)
- **Versions:** 18, 20, 22
- **Startup:** `node /home/container/{{STARTUP}}` (or auto-compiles and runs `.ts`)

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" width="20" height="20"/> Python

- **Egg:** [`egg-python.json`](src/languages/python/egg-python.json)
- **Versions:** 3.9, 3.10, 3.11, 3.12
- **Startup:** `python3 /home/container/{{STARTUP}}`

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
| `STARTUP`     | Main file to run (jar/js/py)       | Varies       | ✅       |
| `SERVER_MEMORY`| Max RAM for Java (e.g. 2048M)     | 2048M        | ✅ (Java) |
| `TZ`          | Timezone                           | UTC          | ❌       |

## 📝 Example Usage

- **Java:**
  - Import `egg-java.json` and set `STARTUP` to your jar file name (e.g. `server.jar`).
  - Set `SERVER_MEMORY` as needed (e.g. `2048M`).
- **Node.js:**
  - Import `egg-node-js.json` and set `STARTUP` to your entry file (e.g. `index.js` or `main.ts`).
- **Python:**
  - Import `egg-python.json` and set `STARTUP` to your main Python file (e.g. `main.py`).

## 🤝 Contributing

1. Fork & branch
2. Add or improve eggs
3. Test on your panel
4. Pull request

## 📜 License

MIT — see [LICENSE](LICENSE)

---

<span style="font-weight:bold;vertical-align:middle;">&#169; 2025 Copyright</span>
<img src="https://img.shields.io/badge/RED%20SHADOWS%20%7C%20RS-DC143C?style=flat&logo=github&logoColor=white&labelColor=2F2F2F" alt="RED SHADOWS | RS" style="vertical-align:middle;"/> &#124; <img src="https://img.shields.io/badge/Shadow--x78-000000?style=flat&logo=github&logoColor=white&labelColor=2F2F2F" alt="Shadow-x78" style="vertical-align:middle;"/> - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
