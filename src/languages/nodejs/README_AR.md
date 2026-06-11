<div align="center" dir="rtl">

# Node.js Egg

تشغيل ملفات JavaScript وTypeScript مع تثبيت الحزم عبر npm.

[![Node.js](https://img.shields.io/badge/Node.js-18%20%7C%2020%20%7C%2022%20%7C%2024-339933?style=flat-square&logo=nodedotjs&logoColor=white)](egg-node-js.json)
[![TypeScript](https://img.shields.io/badge/TypeScript-ts--node-3178C6?style=flat-square&logo=typescript&logoColor=white)](egg-node-js.json)

</div>

---

## 🌐 اللغة

<a href="README.md">🇬🇧 English</a> · <a href="README_AR.md">🇸🇦 العربية</a>

---

## <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" width="16" height="16"> Node.js

| ملف egg | الإصدارات | الملف الافتراضي |
|---------|-----------|-----------------|
| [`egg-node-js.json`](egg-node-js.json) | 18 EOL, 20, 22, 24 | `index.js` |

## 🐳 الصور

| الإصدار | الصورة |
|---------|--------|
| 18 | `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v18` EOL |
| 20 | `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v20` |
| 22 | `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v22` |
| 24 | `ghcr.io/red-shadows-rs/pterodactyl-containers/nodejs:v24` |

## 🚀 التشغيل

```bash
node /home/container/{{STARTUP_FILE}}
```

**المزايا:** تثبيت npm · تشغيل `.js` · تشغيل `.ts` عبر `ts-node`

## ⚙️ المتغيرات

| المتغير | الافتراضي | مطلوب |
|---------|-----------|-------|
| `STARTUP_FILE` | `index.js` | نعم |
| `NODE_PACKAGES` | فارغ | لا |

---

[العودة إلى README الرئيسي](../../../README_AR.md)
