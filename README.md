<div align="center"><img src="https://www.mushoku.eu.cc/waifu/" width="280" alt="AnimeAV1 Waifu">🎌 AnimeAV1

Anime, simplified.

   

Anime API focused on simplicity, speed and clean JSON responses.

🌸 ありがとうございます！ Thanks for visiting AnimeAV1!

</div>
---

✨ Features

Feature	Description

📚 Catalog	Browse the available anime catalog
🔎 Search	Search anime by name
🎬 Episodes	Access anime episodes
🎞️ Anime Information	Detailed information for each anime
📊 MAL / Jikan	Anime metadata through MyAnimeList data
🎧 SUB / DUB	Support for available subtitle and dub information
🚀 REST API	Simple HTTP endpoints returning JSON
💾 Cache	Caching system to reduce unnecessary requests
🛡️ Rate Limit	Protection against excessive requests



---

🌐 Servers

Main Server

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

🔎 Search

GET /buscar/?q=

Example:

https://www.mushoku.eu.cc/buscar/?q=Mushoku%20Tensei

🎬 Anime

GET /anime/{slug}/

Example:

https://www.mushoku.eu.cc/anime/mushoku-tensei/

🎞️ Episode

GET /ep/{slug}/E{numero}/

Example:

https://www.mushoku.eu.cc/ep/mushoku-tensei/E1/

📊 MyAnimeList

GET /mal/{slug}/

Example:

https://www.mushoku.eu.cc/mal/mushoku-tensei/

🆕 Latest Anime

GET /ultimos/

Example:

https://www.mushoku.eu.cc/ultimos/

🔥 Top Anime

GET /top/

Example:

https://www.mushoku.eu.cc/top/

🔤 Anime by Letter

GET /az/{letra}/

Example:

https://www.mushoku.eu.cc/az/a/

📅 Schedule

GET /horario/

Example:

https://www.mushoku.eu.cc/horario/


---

📦 Example Response

{
  "title": "Mushoku Tensei",
  "slug": "mushoku-tensei",
  "episodes": [],
  "status": "Finished Airing",
  "type": "TV",
  "year": 2021
}


---

🛡️ Rate Limit

AnimeAV1 currently limits requests to:

30 requests / minute / IP

This limit helps protect the API and maintain stable performance.


---

⚡ Quick Start

JavaScript

fetch("https://www.mushoku.eu.cc/catalogo/")
  .then(response => response.json())
  .then(data => console.log(data));

PHP

<?php

$url = "https://www.mushoku.eu.cc/catalogo/";
$data = file_get_contents($url);
$json = json_decode($data, true);

print_r($json);


---

🏗️ Built With

🐘 Native PHP

🌐 Apache

📄 .htaccess

🧩 Custom scraper

💾 File-based caching

🚦 Custom rate limiting

🔗 REST-style endpoints

📦 JSON responses


AnimeAV1 uses a custom native PHP backend and does not depend on CakePHP, FuelPHP or another full-stack PHP framework.


---

📁 Project Structure

animeav1/ ├── index.php ├── 404.php ├── anime.php ├── buscar.php ├── catalogo.php ├── ep.php ├── horario.php ├── mal.php ├── top.php ├── ultimos.php ├── az.php ├── cache/ │   └── .htaccess └── src/ ├── RateLimit.php └── Scraper.php


---

🎌 AnimeAV1

AnimeAV1 is designed as a lightweight anime API that can be consumed by websites, applications, players and other projects.

The API focuses on keeping the interface simple:

Request → Processing → JSON

No complicated SDK is required.


---

🔗 Official API

Main:
https://www.mushoku.eu.cc/

Alternate:
http://ww2.mushoku.eu.cc/


---

📜 Usage Policy

AnimeAV1 may be integrated into non-profit projects through the official API.

The API, source code and infrastructure may not be:

Modified

Cloned

Migrated

Self-hosted

Redistributed

Resold

Used commercially

Presented as an independent copy of AnimeAV1


Attribution to AnimeAV1 is required when integrating the API.


---

🐛 Issues & Abuse

For bugs, technical problems or API abuse reports, open an issue in this repository.

Please do not report private information or sensitive data.


---

<div align="center"><img src="https://www.mushoku.eu.cc/waifu/" width="220" alt="Random animated waifu">🌸 AnimeAV1

ありがとうございます！ ✨



Made with ❤️ by iLoveddev

</div>

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
