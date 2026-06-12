<div align="center" dir="rtl">

# Pterodactyl Eggs

ملفات JSON جاهزة للاستيراد داخل Pterodactyl لتشغيل التطبيقات على صور RED SHADOWS من GHCR.

[![Version](https://img.shields.io/badge/version-v11-2563eb?style=flat-square&logo=semver)](CHANGELOG.md)
[![Eggs](https://img.shields.io/badge/eggs-9-16a34a?style=flat-square&logo=json&logoColor=white)](src/)
[![PTDL](https://img.shields.io/badge/PTDL-v2-f59e0b?style=flat-square)](https://pterodactyl.io/)
[![License](https://img.shields.io/badge/license-MIT--NC-dc2626?style=flat-square)](LICENSE)

</div>

---

## 🌐 اللغة

<a href="README.md">🇬🇧 English</a> · <a href="README_AR.md">🇸🇦 العربية</a>

---

## 📋 جدول المحتويات

- [البيض المدعوم](#supported-eggs)
- [خريطة الصور](#image-map)
- [الاستيراد السريع](#quick-import)
- [هيكل المشروع](#project-structure)
- [المساهمة](#contributing)
- [الرخصة](#license)

---

<a id="supported-eggs"></a>
## 🥚 البيض المدعوم

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" width="16" height="16"> Java

| ملف egg | الإصدارات | الصور |
|---------|-----------|-------|
| [`egg-java.json`](src/languages/java/egg-java.json) | 8, 11, 17, 21, 25 | `java:v8` · `java:v11` · `java:v17` · `java:v21` · `java:v25` |

**المزايا:** بناء Maven تلقائي · ملف JAR قابل للتعديل

- - -

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" width="16" height="16"> Node.js

| ملف egg | الإصدارات | الصور |
|---------|-----------|-------|
| [`egg-node-js.json`](src/languages/nodejs/egg-node-js.json) | 18 EOL, 20, 22, 24 | `nodejs:v18` · `nodejs:v20` · `nodejs:v22` · `nodejs:v24` |

**المزايا:** تثبيت npm · تشغيل JavaScript · دعم TypeScript عبر `ts-node`

- - -

### <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" width="16" height="16"> Python

| ملف egg | الإصدارات | الصور |
|---------|-----------|-------|
| [`egg-python.json`](src/languages/python/egg-python.json) | 3.8 EOL, 3.9 EOL, 3.10, 3.11, 3.12, 3.13, 3.14 | `python:v3.8` · `python:v3.9` · `python:v3.10` · `python:v3.11` · `python:v3.12` · `python:v3.13` · `python:v3.14` |

**المزايا:** تحديث pip · تثبيت `requirements.txt` · ملف Python قابل للتعديل

---

## 🌐 أطر الويب

| الإطار | ملف egg | الصورة | المزايا |
|--------|---------|--------|---------|
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" width="14" height="14"> React | [`egg-react.json`](src/frameworks/react/egg-react.json) | `react:latest` | Vite, CRA, scripts مخصصة |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg" width="14" height="14"> Next.js | [`egg-nextjs.json`](src/frameworks/nextjs/egg-nextjs.json) | `nextjs:latest` | npm, pnpm, SSR, SSG |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original.svg" width="14" height="14"> Vue.js | [`egg-vue.json`](src/frameworks/vue/egg-vue.json) | `vue:latest` | Vue CLI, Vite |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original.svg" width="14" height="14"> Angular | [`egg-angular.json`](src/frameworks/angular/egg-angular.json) | `angular:latest` | Angular CLI |

---

## 💻 البرامج

| البرنامج | ملف egg | الصورة | المنفذ الافتراضي |
|----------|---------|--------|------------------|
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" width="14" height="14"> Code-Server | [`egg-code-server.json`](src/softwares/code-server/egg-code-server.json) | `code-server:latest` | `8080` |
| <img src="https://cdn.simpleicons.org/n8n" width="14" height="14"> n8n | [`egg-n8n.json`](src/softwares/n8n/egg-n8n.json) | `n8n:latest` | `5678` |

---

<a id="image-map"></a>
## 🐳 خريطة الصور

كل eggs تستخدم:

```text
ghcr.io/red-shadows-rs/pterodactyl-containers
```

| التصنيف | الصور |
|---------|-------|
| Java | `java:v8` · `java:v11` · `java:v17` · `java:v21` · `java:v25` |
| Node.js | `nodejs:v18` EOL · `nodejs:v20` · `nodejs:v22` · `nodejs:v24` |
| Python | `python:v3.8` EOL · `python:v3.9` EOL · `python:v3.10` · `python:v3.11` · `python:v3.12` · `python:v3.13` · `python:v3.14` |
| الأطر | `react:latest` · `nextjs:latest` · `vue:latest` · `angular:latest` |
| البرامج | `code-server:latest` · `n8n:latest` |

---

<a id="quick-import"></a>
## 🚀 الاستيراد السريع

1. افتح لوحة إدارة Pterodactyl.
2. انتقل إلى **Nests > Import Egg**.
3. ارفع ملف `egg-*.json` المطلوب.
4. اختر الصورة الموجودة داخل egg.
5. اضبط المتغيرات وشغل السيرفر.

---

<a id="project-structure"></a>
## 🏗️ هيكل المشروع

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
## 🤝 المساهمة

1. اعمل fork للمستودع
2. أنشئ branch جديد
3. عدل egg أو README
4. تحقق من JSON
5. افتح Pull Request

---

<a id="license"></a>
## 📜 الرخصة

يوزع المشروع تحت [MIT License (Non-Commercial)](LICENSE).

---

<div align="center" dir="rtl">

بني بواسطة <a href="https://github.com/shadow-x78">SHADOW_x78</a> -
<a href="https://github.com/red-shadows-rs">RED SHADOWS | RS</a> ·
[سجل التغييرات](CHANGELOG.md)

<sub>&copy; 2021 - 2026 RED SHADOWS | RS</sub>

</div>
