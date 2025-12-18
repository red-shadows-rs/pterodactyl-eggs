# Changelog

All notable changes to this project will be documented in this file.

## [v9.2] - 2025-12-18

### 🚀 Added
- **Eggs:** Added Pterodactyl eggs for **Node.js**, **Python**, **Java**, **Vue**, **Angular**, **Next.js**, and **React**.

### 🔄 Updated
- **Documentation:** Complete standardization of all README files.
  - Added specific language/framework badges (Java, Python).
  - Cleaned up Node.js badges (Removed TypeScript badge).
  - Standardized all variable descriptions and startup commands.
- **Node.js:** Renamed egg to "**Node.js**".
- **Java:** Removed explicit memory limits (`-Xmx`) to allow container management.

### 🗑️ Removed
- **Variables:** Removed `SERVER_MEMORY` from Java documentation and configuration.

## [v9.0] - 2025-12-18

### 🚀 Added
- **Web Frameworks:** Added dedicated eggs for **React**, **Next.js**, **Vue.js**, and **Angular**.
  - Optimized startup commands for dev/prod.
  - Included `NODE_PACKAGES` variable for extra dependencies.
  - Native TypeScript support for all Node-based eggs.
- **Node.js:** Native support for TypeScript (`.ts`) files via auto-detected `ts-node` execution.
- **Java:** Added support for **Java 25**.
- **Python:** Added support for **Python 3.13** and **3.14**.

### 🔄 Updated
- **Node.js:** Restored support for **Node 18** (Legacy) alongside 20, 22, and 24.
- **Python:** Restored support for **Python 3.8** and **3.9** (Legacy) alongside 3.10+.
- **Documentation:** Complete overhaul of README files.
  - Standardized "RED SHADOWS | RS" copyright footer.
  - Removed outdated author comments.
  - Added clear "Docker Images" and "Environment Variables" tables.
- **Installation:** Updated all install scripts to be more robust (global `ts-node`, `typescript`, `@types/node` for Node eggs; `openjdk-25-jdk` for Java).

### 🗑️ Removed
- **Variables:** Removed `Timezone` (TZ) and `Git Repository` (INSTALL_REPO) variables from all eggs to simplify configuration.

## [v8.0] - 2025-06-23

### 🚀 Added
- **Java:** Added support for **Java 21** (LTS).
- **Node.js:** Added support for **Node.js 22**.
- **Python:** Added support for **Python 3.12**.
- **Docker:** Updated base images to use `bookworm` and `bullseye` variants for better stability.

## [v6.5] - 2025-01-15

### 🔄 Changed
- **Standardization:** Unified the startup variable name to `STARTUP_FILE` across all languages (Java, Node, Python) to ensure consistency.
- **Documentation:** Added badges and clearer instruction tables to READMEs.

## [v1.0] - 2024-08-01

### 🎉 Initial Release
- **Launch:** Initial release of Pterodactyl Eggs.
- **Support:** Basic support for:
  - Java 8, 11, 17
  - Node.js 18, 20
  - Python 3.9, 3.10, 3.11
- **Features:** Automated installation scripts and basic environment variables.
