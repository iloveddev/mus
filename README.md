<div align="center">

<img src="https://is.wuaze.com/static/icon/Icon.png" width="120" alt="AnimeAV1 Logo">

# AnimeAV1 API

### 🎌 Anime API · Jikan/MAL · SUB & DUB · JSON

[![API](https://img.shields.io/badge/API-Online-ff6b9d?style=for-the-badge)](https://www.mushoku.eu.cc/)
[![PHP](https://img.shields.io/badge/PHP-Native-777bb4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![License](https://img.shields.io/badge/License-Custom-ff9f43?style=for-the-badge)](#-licencia)

<br>

**AnimeAV1** es una API ligera de anime creada para proyectos, aplicaciones y sitios relacionados con anime.

[🌐 API](https://www.mushoku.eu.cc/) · [📚 Documentación](#-endpoints) · [🐛 Reportar problema](../../issues)

</div>

---

## ✨ Sobre AnimeAV1

AnimeAV1 proporciona información de anime en formato **JSON**, incluyendo información basada en **MyAnimeList/Jikan**, episodios, búsqueda, rankings y más.

Está diseñada para ser sencilla de integrar en aplicaciones web, aplicaciones móviles y otros proyectos relacionados con anime.

### 🌸 Características

- 🎌 Información de anime
- 🔎 Búsqueda por nombre
- 📺 Episodios
- 🎙️ SUB / DUB
- ⭐ Rankings
- 📅 Horarios
- 🔤 Búsqueda por letra
- 🆔 Información de MyAnimeList
- ⚡ Sistema de caché
- 🚦 Rate limit
- 📦 Respuestas JSON
- 🪶 Backend ligero en PHP nativo

---

## 🌐 Servidores

### Servidor principal

https://www.mushoku.eu.cc/

### Servidor alternativo

http://ww2.mushoku.eu.cc/

> El servidor alternativo está previsto como respaldo y puede no estar disponible permanentemente.

---

# 📚 Endpoints

Todos los endpoints devuelven información en formato **JSON** salvo cuando se indique lo contrario.

## 📦 Catálogo

GET /catalogo/

Obtiene el catálogo disponible de anime.

Ejemplo:
https://www.mushoku.eu.cc/catalogo/

---

## 🔎 Buscar anime

GET /buscar/?q={consulta}

Busca anime mediante una consulta.

Ejemplo:
https://www.mushoku.eu.cc/buscar/?q=Mushoku%20Tensei

---

## 🎬 Información de anime

GET /anime/{slug}/

Obtiene información detallada de un anime.

Ejemplo:
https://www.mushoku.eu.cc/anime/mushoku-tensei/

---

## ▶️ Episodio

GET /ep/{slug}/E{numero}/

Obtiene información correspondiente a un episodio.

Ejemplo:
https://www.mushoku.eu.cc/ep/mushoku-tensei/E1/

---

## 🇲🇽 MyAnimeList

GET /mal/{slug}/

Obtiene información relacionada con MyAnimeList.

Ejemplo:
https://www.mushoku.eu.cc/mal/mushoku-tensei/

---

## 🆕 Últimos lanzamientos

GET /ultimos/

Obtiene los últimos anime o episodios disponibles.

Ejemplo:
https://www.mushoku.eu.cc/ultimos/

---

## 🔥 Top anime

GET /top/

Obtiene el ranking de anime.

Ejemplo:
https://www.mushoku.eu.cc/top/

---

## 🔤 Anime por letra

GET /az/{letra}/

Obtiene anime que comienzan con una letra determinada.

Ejemplo:
https://www.mushoku.eu.cc/az/A/

---

## 📅 Horario

GET /horario/

Obtiene información del horario de emisión.

Ejemplo:
https://www.mushoku.eu.cc/horario/

---

# 📄 Formato de respuesta

AnimeAV1 utiliza **JSON** para las respuestas de la API.

Ejemplo conceptual:

{
  "title": "Mushoku Tensei",
  "episodes": 23,
  "status": "Finished Airing"
}

La estructura exacta puede variar dependiendo del endpoint.

---

# 🚦 Rate Limit

30 solicitudes por minuto / IP

Si superas el límite, espera antes de realizar nuevas solicitudes.

---

# 🛠️ Tecnología

AnimeAV1 utiliza un backend ligero basado en:

- PHP nativo
- Apache
- .htaccess
- JSON
- Sistema de caché
- Jikan / MyAnimeList

No utiliza CakePHP ni FuelPHP.

---

# 📌 Política de uso

AnimeAV1 puede utilizarse gratuitamente para integrar información de anime en proyectos **sin fines de lucro**.

### ✅ Permitido

- Integrar la API en proyectos personales.
- Utilizarla en aplicaciones gratuitas.
- Utilizarla mediante tu propio dominio oficial.
- Crear interfaces que consuman AnimeAV1.

### ❌ No permitido

- Clonar AnimeAV1.
- Copiar o modificar el backend.
- Migrar el backend a otro servidor.
- Autohospedar una copia de la API.
- Redistribuir el código fuente.
- Revender la API.
- Utilizarla como servicio comercial sin autorización.
- Hacer pasar una copia modificada como AnimeAV1.

---

# 🧩 Atribución

Si utilizas AnimeAV1 en un proyecto, se recomienda mantener una referencia a:

AnimeAV1 API
https://www.mushoku.eu.cc/

No es necesario colocar publicidad.

---

# 🐛 Issues & abuso

Si encuentras:

- errores
- endpoints caídos
- respuestas incorrectas
- problemas de seguridad
- abuso del servicio

puedes abrir un **Issue** en este repositorio.

Por favor, evita realizar spam o solicitudes masivas que puedan afectar al servicio.

---

# 📜 Licencia

AnimeAV1 utiliza una **licencia personalizada**.

El acceso a la API puede utilizarse gratuitamente en proyectos no comerciales, pero el código y la infraestructura no pueden copiarse, modificarse, migrarse, clonarse, redistribuirse o alojarse por terceros sin autorización.

El uso comercial requiere autorización previa.

---

# 💗 Thanks for Visiting

<div align="center">

### Gracias por visitar AnimeAV1 ♡

<img src="https://count.getloli.com/@animeav1?name=animeav1&theme=flat&padding=7&offset=253&align=center&scale=1&pixelated=1" alt="AnimeAV1 visitor counter">

<br><br>

<img src="https://github-readme-utils.vercel.app/api/gif/anime" width="220" alt="Random anime waifu">

<br>

### またね！ ✨

</div>

---

<div align="center">

### 🎌 AnimeAV1

**Made with ❤️ for anime projects**

<img src="https://img.shields.io/badge/Anime-AV1-ff6b9d?style=flat-square">

<br><br>

⭐ If AnimeAV1 is useful for your project, consider giving this repository a star.

</div>
### 🔥 Top Anime

GET /top/

Example:
https://www.mushoku.eu.cc/top/

### 🔤 Alphabetical Search

GET /az/{letter}/

Example:
https://www.mushoku.eu.cc/az/a/

### 📅 Schedule

GET /horario/

Example:
https://www.mushoku.eu.cc/horario/

---

## 📦 Response Format

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

## ⚡ Rate Limits

AnimeAV1 API currently applies a rate limit of:

30 requests / minute / IP

Please avoid excessive requests and respect the API infrastructure.

Attempts to bypass rate limits or intentionally overload the service may result in access restrictions.

---

## 🚀 Quick Start

You can request an endpoint directly from your application.

### JavaScript

fetch("https://www.mushoku.eu.cc/catalogo/")
  .then(response => response.json())
  .then(data => {
    console.log(data);
  });

### PHP

<?php

$response = file_get_contents(
    "https://www.mushoku.eu.cc/catalogo/"
);

$data = json_decode($response, true);

print_r($data);

---

## 🛠️ Built With

PHP — Native
Apache — .htaccess
REST API

AnimeAV1 is built using native PHP, without CakePHP, FuelPHP, or another PHP framework.

The project uses Apache .htaccess rules for routing and access handling.

---

## 📁 Project Structure

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

## 🔐 Usage Policy

AnimeAV1 API is intended for free integration into non-profit projects.

### ✅ Allowed

You may:

- Integrate the API into non-profit applications and websites.
- Use API responses within your own project.
- Create interfaces that consume the API.
- Use the API for personal, educational or community projects.

### ❌ Not Allowed

Without explicit permission from iLoveddev, you may not:

- Modify the AnimeAV1 API source code.
- Clone, mirror or migrate the API.
- Self-host or redistribute the API.
- Create an alternative API based on AnimeAV1.
- Resell access to the API.
- Use the API for commercial purposes.
- Proxy or relay the API under another domain.
- Bypass rate limits or security restrictions.
- Impersonate AnimeAV1 or iLoveddev.
- Present AnimeAV1's infrastructure or code as your own.

> The API is provided for integration, not migration or redistribution.

---

## 📌 Attribution

If your project uses AnimeAV1 API, attribution is appreciated:

> Powered by AnimeAV1 API — by iLoveddev.

---

## 🐛 Issues & Abuse

If you find a bug, security issue or abuse involving the API, please report it through the repository's Issues section.

Please do not intentionally exploit vulnerabilities or intentionally overload the API.

---

## 📜 License

AnimeAV1 API is distributed under a custom usage license.

See LICENSE for the complete terms and restrictions.

---

## 🌸 Thanks for Visiting

<div align="center">

<img src="https://is.wuaze.com/static/icon/Icon.png" width="90" alt="AnimeAV1">

### 🎁 AnimeAV1

**Made with ❤️ by iLoveddev**

アニメを、もっとシンプルに。 ✨

<br>

<img src="https://anime-counter.lulushu.workers.dev/@animeav1?theme=naruto&pixelated=1&scale=1" alt="AnimeAV1 visitor counter">

<br><br>

<img src="./assets/waifu.gif" width="220" alt="AnimeAV1 waifu">

<br><br>

<sub>🌸 Thanks for visiting AnimeAV1!</sub>

<br>

<sub>ありがとうございます！ ✨</sub>

</div>

---

<div align="center">

**AnimeAV1 — Anime, simplified.**

</div>
Example:

https://www.mushoku.eu.cc/az/a/

### 📅 Schedule

`GET /horario/`

Example:

https://www.mushoku.eu.cc/horario/

---

## 📦 Example Response

```json
{
  "title": "Mushoku Tensei",
  "slug": "mushoku-tensei",
  "episodes": [],
  "status": "Finished Airing",
  "type": "TV",
  "year": 2021
}
```

---

## 🛡️ Rate Limit

AnimeAV1 currently limits requests to:

`30 requests / minute / IP`

This limit helps protect the API and maintain stable performance.

---

## ⚡ Quick Start

### JavaScript

```js
fetch("https://www.mushoku.eu.cc/catalogo/")
  .then(response => response.json())
  .then(data => console.log(data));
```

### PHP

```php
<?php

$url = "https://www.mushoku.eu.cc/catalogo/";
$data = file_get_contents($url);
$json = json_decode($data, true);

print_r($json);
```

---

## 🏗️ Built With

- 🐘 Native PHP
- 🌐 Apache
- 📄 `.htaccess`
- 🧩 Custom scraper
- 💾 File-based caching
- 🚦 Custom rate limiting
- 🔗 REST-style endpoints
- 📦 JSON responses

AnimeAV1 uses a **custom native PHP backend** and does not depend on CakePHP, FuelPHP or another full-stack PHP framework.

---

## 📁 Project Structure

```text
animeav1/
├── index.php
├── 404.php
├── anime.php
├── buscar.php
├── catalogo.php
├── ep.php
├── horario.php
├── mal.php
├── top.php
├── ultimos.php
├── az.php
├── cache/
│   └── .htaccess
└── src/
    ├── RateLimit.php
    └── Scraper.php
```

---

## 🎌 AnimeAV1

AnimeAV1 is designed as a lightweight anime API that can be consumed by websites, applications, players and other projects.

The API focuses on keeping the interface simple:

`Request → Processing → JSON`

No complicated SDK is required.

---

## 📜 Usage Policy

AnimeAV1 may be integrated into non-profit projects through the official API.

The API, source code and infrastructure may not be:

- Modified
- Cloned
- Migrated
- Self-hosted
- Redistributed
- Resold
- Used commercially
- Presented as an independent copy of AnimeAV1

Attribution to AnimeAV1 is required when integrating the API.

---

## 🐛 Issues & Abuse

For bugs, technical problems or API abuse reports, open an issue in this repository.

Please do not report private information or sensitive data.

---

<div align="center">

<img src="https://www.mushoku.eu.cc/waifu/" width="240" alt="Random animated waifu">

### 🌸 AnimeAV1

ありがとうございます！ ✨

![Visitors](https://anime-counter.lulushu.workers.dev/@animeav1?theme=waifu&pixelated=1&scale=1)

**Made with ❤️ by iLoveddev**

</div>
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
