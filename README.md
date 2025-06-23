<!-- © Copyright RED SHADOWS | RS - Shadow-x78 -->

# Pterodactyl Eggs 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-eggs-blue?style=for-the-badge&logo=json&logoColor=white)
<<<<<<< HEAD
=======
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
>>>>>>> 3055eabd266858b909923daccd06d2837f0251ab

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured eggs for popular languages
- 🛠️ **Easy import**: One-click import into Pterodactyl panel
- 🔒 **Secure**: Minimal, safe startup commands
- 🧩 **Customizable**: Edit variables and startup as needed
- 📝 **Well-documented**: Clear instructions for each egg

## 🐣 Supported Eggs

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="Java" width="20" height="20"/> Java

- **Egg:** [`egg-java.json`](Java/egg-java.json)
- **Versions:** 8, 11, 17, 21
- **Startup:** `java -Xms128M -Xmx{{SERVER_MEMORY}}M -jar {{SERVER_JARFILE}}`

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" alt="Node.js" width="20" height="20"/> Node.js

- **Egg:** [`egg-node-js.json`](Nodejs/egg-node-js.json)
- **Versions:** 18, 20, 22
- **Startup:** `{{STARTUP_CMD}}`

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" width="20" height="20"/> Python

- **Egg:** [`egg-python.json`](Python/egg-python.json)
- **Versions:** 3.9, 3.10, 3.11, 3.12
- **Startup:** `python3 {{SERVER_FILE}}`

## 📥 Importing Eggs

1. Go to your Pterodactyl admin panel
2. Navigate to **Nests → Import Egg**
3. Upload the desired `egg-*.json` file from this repo
4. Configure variables as needed
5. Assign the egg to a server

> **Tip:** Each egg comes with recommended Docker images. See the [Pterodactyl Containers](../README.md) for compatible images.

## ⚙️ Environment Variables

| Variable        | Description                | Default         | Required |
|-----------------|---------------------------|-----------------|----------|
| `SERVER_JARFILE`| Main JAR file (Java)      | `server.jar`    | ✅       |
| `STARTUP_CMD`   | Node.js start command     | `node index.js` | ✅       |
| `SERVER_FILE`   | Python entry file         | `main.py`       | ✅       |
| `TZ`            | Timezone                  | `UTC`           | ❌       |

## 📝 Example Usage

- **Java:**
  - Import `egg-java.json` and set `SERVER_JARFILE` to your jar file name.
- **Node.js:**
  - Import `egg-node-js.json` and set `STARTUP_CMD` to your start script.
- **Python:**
  - Import `egg-python.json` and set `SERVER_FILE` to your main Python file.

## 🤝 Contributing

1. Fork & branch
2. Add or improve eggs
3. Test on your panel
4. Pull request

## 📜 License

MIT — see [LICENSE](../LICENSE)

---

<span style="font-weight:bold;vertical-align:middle;">&#169; 2025 Copyright</span>
<<<<<<< HEAD
<img src="https://img.shields.io/badge/RED%20SHADOWS%20%7C%20RS-DC143C?style=flat&logo=github&logoColor=white&labelColor=2F2F2F" alt="RED SHADOWS | RS" style="vertical-align:middle;"/> &#124; <img src="https://img.shields.io/badge/Shadow--x78-000000?style=flat&logo=github&logoColor=white&labelColor=2F2F2F" alt="Shadow-x78" style="vertical-align:middle;"/> - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
=======
<img src="https://img.shields.io/badge/RED%20SHADOWS%20%7C%20RS-DC143C?style=flat&logo=github&logoColor=white&labelColor=2F2F2F" alt="RED SHADOWS | RS" style="vertical-align:middle;"/> &#124; <img src="https://img.shields.io/badge/Shadow--x78-000000?style=flat&logo=github&logoColor=white&labelColor=2F2F2F" alt="Shadow-x78" style="vertical-align:middle;"/> - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
>>>>>>> 3055eabd266858b909923daccd06d2837f0251ab
