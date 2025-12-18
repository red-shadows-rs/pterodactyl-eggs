# Java Pterodactyl Egg 🥚

![Pterodactyl](https://img.shields.io/badge/Pterodactyl-0e4688?style=for-the-badge&logo=pterodactyl&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

## ✨ Features

- 📦 **Ready-to-use**: Pre-configured for Java applications
- 🛠️ **Easy import**: One-click import into Pterodactyl panel
- 🔒 **Secure**: Minimal, safe startup commands
- 🧩 **Customizable**: Edit variables and startup as needed
- 📝 **Well-documented**: Clear instructions and variables

## 🐣 Supported Versions

- **Java 25**
- **Java 21**
- **Java 17**
- **Java 11**
- **Java 8**

## 🚀 Startup Command

```bash
java -Xms128M -jar /home/container/{{STARTUP_FILE}}
```

- Automatically runs `mvn clean install` if a `pom.xml` is found before starting the JAR.
- Shows an error if the JAR file is missing.

## 🐳 Docker Images

- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v25`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v21`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v17`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v11`
- `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v8`

## ⚙️ Environment Variables

| Variable         | Description                        | Default      | Required |
|------------------|------------------------------------|--------------|----------|
| `STARTUP_FILE`   | The main file to start the server (e.g. server.jar). | server.jar   | ✅       |

## 📝 Example Usage

- Import `egg-java.json` in your Pterodactyl panel.
- Set `STARTUP_FILE` to your JAR file name (e.g. `server.jar`).
- Start your server!

## 🛠️ Installation Script

Installs all required Java versions and build tools:

```bash
apt update
apt install -y curl jq file unzip git maven openjdk-8-jdk openjdk-11-jdk openjdk-17-jdk openjdk-21-jdk openjdk-25-jdk
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
**RED SHADOWS | RS** - <span style="font-weight:bold;vertical-align:middle;">All rights reserved</span>
