# MUS API V1! 
<div align="center"><img src="https://is.wuaze.com/static/icon/Icon.png" alt="AnimeAV1" width="150">AnimeAV1 API

🎌 A simple, fast and free Anime API built with PHP.

<p>
  <img src="https://img.shields.io/badge/PHP-Native-777BB4?style=for-the-badge&logo=php&logoColor=white">
  <img src="https://img.shields.io/badge/API-REST-00A98F?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Online-success?style=for-the-badge">
</p><p>
  <a href="https://www.mushoku.eu.cc/">🌐 API</a>
  •
  <a href="https://www.mushoku.eu.cc/catalogo/">📚 Catalog</a>
  •
  <a href="https://www.mushoku.eu.cc/ultimos/">🆕 Latest</a>
  •
  <a href="https://www.mushoku.eu.cc/top/">🔥 Top</a>
</p><br><img src="https://count.getloli.com/@animeav1?name=animeav1&theme=booru-r6&padding=7&offset=0&align=center&scale=1&pixelated=1&darkmode=auto" alt="AnimeAV1 Visitors"><br><br>

<img src="https://media.tenor.com/3XqKJvGmV4AAAAAC/anime-girl.gif" width="150" alt="Anime Waifu"><br><sub>🌸 Thanks for visiting AnimeAV1!</sub>

<br><sub>ありがとうございます！ ✨</sub>

</div>---

<div align="center">«🎌 AnimeAV1 — Anime, simplified.»

A lightweight PHP API designed to provide anime information, episodes, servers and additional metadata through a simple REST interface.

</div>---

✨ Features

| Feature
🎌| Anime catalog
🔎| Anime search
📺| Episodes & streaming servers
⭐| MyAnimeList information
🏷️| Genres, status and metadata
🆕| Recently added anime
🔥| Popular / top anime
🔤| Alphabetical browsing
📅| Anime schedule
⚡| Response caching
🛡️| IP-based rate limiting
🐘| Native PHP backend

---

🌐 Official Servers

🟢 Main Server

https://www.mushoku.eu.cc/

The primary and officially supported AnimeAV1 API server.

🟡 Alternate Server

http://ww2.mushoku.eu.cc/

Coming soon.

The alternate server is intended to provide additional availability when it becomes operational.

«⚠️ Only domains officially provided by AnimeAV1 / iLoveddev should be considered official API servers.»

---

📡 API Endpoints

📚 Catalog

GET /catalogo/

Returns the available anime catalog.

---

🔎 Search

GET /buscar/?q=naruto

Search for anime by name.

---

🎌 Anime Information

GET /anime/{slug}/

Returns information about a specific anime.

Example:

/anime/mushoku-tensei/

---

📺 Episode

GET /ep/{slug}/E{number}/

Returns information about a specific episode, including available streaming servers.

Example:

/ep/mushoku-tensei/E01/

---

⭐ MyAnimeList

GET /mal/{slug}/

Returns additional MyAnimeList-related information for an anime.

---

🆕 Latest Anime

GET /ultimos/

Returns recently added anime.

---

🔥 Top Anime

GET /top/

Returns popular/top anime.

---

🔤 Alphabetical Index

GET /az/{letter}/

Browse anime alphabetically.

Example:

/az/a/

---

📅 Schedule

GET /horario/

Returns the anime release schedule.

---

📦 Response Format

AnimeAV1 API returns structured data primarily in JSON.

Example:

{
  "title": "Mushoku Tensei",
  "slug": "mushoku-tensei",
  "episodes": 24,
  "status": "Completed"
}

«The exact response structure may vary depending on the endpoint and available data.»

---

⚡ Rate Limits

AnimeAV1 API currently applies a rate limit of:

30 requests / minute / IP

Please avoid excessive requests and respect the API infrastructure.

Attempts to bypass rate limits or intentionally overload the service may result in access restrictions.

---

🚀 Quick Start

You can request an endpoint directly from your application.

JavaScript

fetch("https://www.mushoku.eu.cc/catalogo/")
  .then(response => response.json())
  .then(data => {
    console.log(data);
  });

PHP

<?php

$url = "https://www.mushoku.eu.cc/catalogo/";

$response = file_get_contents($url);
$data = json_decode($response, true);

print_r($data);

---

🛠️ Built With

<div align="center"><img src="https://img.shields.io/badge/PHP-Native-777BB4?style=for-the-badge&logo=php&logoColor=white">
<img src="https://img.shields.io/badge/Apache-.htaccess-D22128?style=for-the-badge&logo=apache&logoColor=white">
<img src="https://img.shields.io/badge/REST-API-00A98F?style=for-the-badge"></div>AnimeAV1 is built using native PHP, without CakePHP, FuelPHP, or another PHP framework.

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
│
└── .htaccess

---

🔐 Usage Policy

AnimeAV1 API is intended for free integration into non-profit projects.

✅ Allowed

You may:

- Integrate the API into non-profit applications and websites.
- Use API responses within your own project.
- Create interfaces that consume the API.
- Use the API for personal, educational or community projects.

❌ Not Allowed

Without explicit permission from iLoveddev, you may not:

- Modify the API source code.
- Clone, mirror or migrate the API.
- Self-host or redistribute the API.
- Create an alternative API based on AnimeAV1.
- Resell access to the API.
- Use the API for commercial purposes.
- Proxy or mirror the API under another domain.
- Bypass rate limits or security restrictions.
- Impersonate AnimeAV1 or iLoveddev.
- Present AnimeAV1's infrastructure or code as your own.

«The API is provided for integration, not migration or redistribution.»

---

📌 Attribution

If your project uses AnimeAV1 API, attribution is appreciated:

Powered by AnimeAV1 API — by iLoveddev

---

🐛 Issues & Abuse

If you find a bug, security issue or abuse involving the API, please report it through the repository's Issues section.

Please do not intentionally exploit vulnerabilities or overload the API.

---

📜 License

AnimeAV1 API is distributed under a custom usage license.

See ""LICENSE"" (LICENSE) for the complete terms and restrictions.

---

<br><div align="center"><img src="https://is.wuaze.com/static/icon/Icon.png" alt="AnimeAV1" width="65">🌸 AnimeAV1

Made with ❤️ by iLoveddev

<br><sub>アニメを、もっとシンプルに。 ✨</sub>

<br><br>

<img src="https://count.getloli.com/@animeav1?name=animeav1&theme=booru-r6&padding=7&offset=0&align=center&scale=1&pixelated=1&darkmode=auto" alt="AnimeAV1 Visitor Counter"><br><br>

<sub>© 2026 iLoveddev — AnimeAV1 API</sub>

</div>
