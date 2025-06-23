<!-- © Copyright RED SHADOWS | RS - Shadow-x78 -->

# Java Pterodactyl Egg 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-egg-blue?style=for-the-badge&logo=json&logoColor=white)

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured for Java applications
- 🛠️ **Easy import**: One-click import into Pterodactyl panel
- 🔒 **Secure**: Minimal, safe startup commands
- 🧩 **Customizable**: Edit variables and startup as needed
- 📝 **Well-documented**: Clear instructions and variables

## 🐣 Supported Versions

- **Java 8**
- **Java 11**
- **Java 17**
- **Java 21**

## 🚀 Startup Command

```bash
java -Xms128M -Xmx{{SERVER_MEMORY}} -jar /home/container/{{STARTUP_FILE}}
```

- Automatically runs `mvn clean install` if a `pom.xml` is found before starting the JAR.
- Shows an error if the JAR file is missing.

## 🐳 Docker Images

- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v21`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v17`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v11`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v8`

## ⚙️ Environment Variables

| Variable         | Description                        | Default      | Required |
|------------------|------------------------------------|--------------|----------|
| `STARTUP_FILE`   | Main JAR file name (e.g. server.jar)| server.jar   | ✅       |
| `SERVER_MEMORY`  | Maximum RAM for Java (e.g. 2048M)   | 2048M        | ✅       |
| `TZ`             | Timezone                            | UTC          | ❌       |

## 📝 Example Usage

- Import `egg-java.json` in your Pterodactyl panel.
- Set `STARTUP_FILE` to your JAR file name (e.g. `server.jar`).
- Set `SERVER_MEMORY` as needed (e.g. `2048M`).
- Start your server!

## 🛠️ Installation Script

Installs all required Java versions and build tools:

```bash
apt update
apt install -y curl jq file unzip git maven openjdk-8-jdk openjdk-11-jdk openjdk-17-jdk openjdk-21-jdk
```

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
