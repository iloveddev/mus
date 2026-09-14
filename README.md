<div align="center">

<img src="https://is.wuaze.com/static/icon/Icon.png" width="120" alt="AnimeAV1">

# AnimeAV1 API

**Anime, simplified.** 🌸

A lightweight anime API built with native PHP.

<br>

[![PHP](https://img.shields.io/badge/PHP-Native-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![API](https://img.shields.io/badge/REST-API-00A98F?style=for-the-badge)](#-endpoints)
[![Apache](https://img.shields.io/badge/Apache-.htaccess-D22128?style=for-the-badge&logo=apache&logoColor=white)](#%EF%B8%8F-built-with)
[![Status](https://img.shields.io/badge/Status-Online-2ea44f?style=for-the-badge)](https://www.mushoku.eu.cc/)

<br>

[🌐 API](https://www.mushoku.eu.cc/) •
[📚 Catalog](https://www.mushoku.eu.cc/catalogo/) •
[🆕 Latest](https://www.mushoku.eu.cc/ultimos/) •
[🔥 Top](https://www.mushoku.eu.cc/top/)

</div>

---

## ✨ Features

| Feature | Description |
|---|---|
| ⚡ Lightweight | Built with native PHP |
| 📚 Anime Catalog | Access the available anime catalog |
| 🔎 Search | Search anime by name |
| 🎬 Episodes | Access episode information |
| 🇯🇵 MAL / Jikan | Anime metadata through MyAnimeList data |
| 🎧 SUB / DUB | Support for available subtitle and dub information |
| 🚀 REST API | Simple HTTP endpoints returning JSON |
| 💾 Cache | Caching system to reduce unnecessary requests |
| 🛡️ Rate Limit | Protection against excessive requests |

---

## 🌐 Servers

### Main Server

```text
https://www.mushoku.eu.cc/

Alternate Server

http://ww2.mushoku.eu.cc/


---

📡 Endpoints

All endpoints return JSON data.

📚 Catalog

GET /catalogo/

Example:

https://www.mushoku.eu.cc/catalogo/


---

🔎 Search

GET /buscar/?q={query}

Example:

https://www.mushoku.eu.cc/buscar/?q=mushoku+tensei


---

🎬 Anime

GET /anime/{slug}/

Example:

https://www.mushoku.eu.cc/anime/mushoku-tensei/


---

▶️ Episode

GET /ep/{slug}/E{number}/

Example:

https://www.mushoku.eu.cc/ep/mushoku-tensei/E1/


---

⭐ MyAnimeList

GET /mal/{slug}/

Example:

https://www.mushoku.eu.cc/mal/mushoku-tensei/


---

🆕 Latest Releases

GET /ultimos/

Example:

https://www.mushoku.eu.cc/ultimos/


---

🔥 Top Anime

GET /top/

Example:

https://www.mushoku.eu.cc/top/


---

🔤 Alphabetical Search

GET /az/{letter}/

Example:

https://www.mushoku.eu.cc/az/a/


---

📅 Schedule

GET /horario/

Example:

https://www.mushoku.eu.cc/horario/


---

📦 Response Format

AnimeAV1 uses JSON responses.

Example:

{
  "title": "Mushoku Tensei",
  "slug": "mushoku-tensei",
  "episodes": [
    {
      "number": 1,
      "title": "Episode 1"
    }
  ]
}

The exact response structure may vary depending on the endpoint.


---

⚡ Rate Limits

AnimeAV1 API currently applies a rate limit of:

30 requests / minute / IP

Please avoid excessive requests and respect the API infrastructure.

Attempts to bypass rate limits or intentionally overload the service may result in access restrictions.


---

🚀 Quick Start

JavaScript

fetch("https://www.mushoku.eu.cc/catalogo/")
  .then(response => response.json())
  .then(data => {
    console.log(data);
  });

PHP

<?php

$response = file_get_contents(
    "https://www.mushoku.eu.cc/catalogo/"
);

$data = json_decode($response, true);

print_r($data);


---

🛠️ Built With

<div align="center">  

</div>AnimeAV1 is built using native PHP, without CakePHP, FuelPHP, or another PHP framework.

The project uses Apache .htaccess rules for routing and access handling.


---

📁 Project Structure

animeav1-api/
│
├── src/
│   ├── RateLimit.php
│   └── Scraper.php
│
├── cache/
│   └── .htaccess
│
├── anime.php
├── catalogo.php
├── buscar.php
├── ep.php
├── mal.php
├── ultimos.php
├── top.php
├── az.php
├── horario.php
├── index.php
├── 404.php
└── .htaccess


---

🔐 Usage Policy

AnimeAV1 API is intended for free integration into non-profit projects.

✅ Allowed

You may:

Integrate the API into non-profit applications and websites.

Use API responses within your own project.

Create interfaces that consume the API.

Use the API for personal, educational or community projects.


❌ Not Allowed

Without explicit permission from iLoveddev, you may not:

Modify the AnimeAV1 API source code.

Clone, mirror or migrate the API.

Self-host or redistribute the API.

Create an alternative API based on AnimeAV1.

Resell access to the API.

Use the API for commercial purposes.

Proxy or relay the API under another domain.

Bypass rate limits or security restrictions.

Impersonate AnimeAV1 or iLoveddev.

Present AnimeAV1's infrastructure or code as your own.


> The API is provided for integration, not migration or redistribution.




---

📌 Attribution

If your project uses AnimeAV1 API, attribution is appreciated:

> Powered by AnimeAV1 API — by iLoveddev.




---

🐛 Issues & Abuse

If you find a bug, security issue or abuse involving the API, please report it through the repository's Issues section.

Please do not intentionally exploit vulnerabilities or intentionally overload the API.


---

📜 License

AnimeAV1 API is distributed under a custom usage license.

See LICENSE for the complete terms and restrictions.


---

🌸 Thanks for Visiting

<div align="center"><img src="https://is.wuaze.com/static/icon/Icon.png" width="90" alt="AnimeAV1">🎁 AnimeAV1

Made with ❤️ by iLoveddev

アニメを、もっとシンプルに。 ✨

<br><img src="https://anime-counter.lulushu.workers.dev/@animeav1?theme=naruto&pixelated=1&scale=1" alt="AnimeAV1 visitor counter"><br><br>

<img src="https://www.mushoku.eu.cc/waifu/" width="300" alt="Random animated waifu"><br><br>

<sub>🌸 Thanks for visiting AnimeAV1!</sub>

<br><sub>ありがとうございます！ ✨</sub>

</div>
---

<div align="center">AnimeAV1 — Anime, simplified.

</div>
```
