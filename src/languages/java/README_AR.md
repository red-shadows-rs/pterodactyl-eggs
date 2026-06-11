<div align="center" dir="rtl">

# Java Egg

تشغيل تطبيقات Java بصيغة JAR مع دعم بناء Maven عند الحاجة.

[![Java](https://img.shields.io/badge/Java-8%20%7C%2011%20%7C%2017%20%7C%2021%20%7C%2025-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](egg-java.json)
[![PTDL](https://img.shields.io/badge/PTDL-v2-f59e0b?style=flat-square)](egg-java.json)

</div>

---

## 🌐 اللغة

<a href="README.md">🇬🇧 English</a> · <a href="README_AR.md">🇸🇦 العربية</a>

---

## ☕ Java

| ملف egg | الإصدارات | الملف الافتراضي |
|---------|-----------|-----------------|
| [`egg-java.json`](egg-java.json) | 8, 11, 17, 21, 25 | `server.jar` |

## 🐳 الصور

| الإصدار | الصورة |
|---------|--------|
| 8 | `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v8` |
| 11 | `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v11` |
| 17 | `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v17` |
| 21 | `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v21` |
| 25 | `ghcr.io/red-shadows-rs/pterodactyl-containers/java:v25` |

## 🚀 التشغيل

```bash
java -Xms128M -jar /home/container/{{STARTUP_FILE}}
```

**المزايا:** فحص ملف JAR · بناء Maven عند وجود `pom.xml`

## ⚙️ المتغيرات

| المتغير | الافتراضي | مطلوب |
|---------|-----------|-------|
| `STARTUP_FILE` | `server.jar` | نعم |

---

[العودة إلى README الرئيسي](../../../README_AR.md)
