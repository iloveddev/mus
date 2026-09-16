<div align="center"><img src="https://is.wuaze.com/static/icon/Icon.png" width="120" alt="AnimeAV1 Logo">AnimeAV1 API

🎌 Anime API · Jikan/MAL · SUB & DUB · JSON

""API" (https://img.shields.io/badge/API-Online-ff6b9d?style=for-the-badge)" (https://www.mushoku.eu.cc/)
""PHP" (https://img.shields.io/badge/PHP-Native-777bb4?style=for-the-badge&logo=php&logoColor=white)" (https://www.php.net/)
""License" (https://img.shields.io/badge/License-Custom-ff9f43?style=for-the-badge)" (#-licencia)

<br>AnimeAV1 es una API ligera de anime creada para proyectos, aplicaciones y sitios relacionados con anime.

"🌐 API" (https://www.mushoku.eu.cc/) · "📚 Documentación" (#-endpoints) · "🐛 Reportar problema" (../../issues)

</div>---

📚 Catálogo

«Obtiene los animes disponibles en el catálogo de AnimeAV1.»

🔗 Endpoint

GET /catalogo/

⚙️ Parámetros

Parámetro| Tipo| Descripción
"page"| "int"| Página del catálogo
"genre"| "string"| Filtrar por género
"search"| "string"| Filtrar por búsqueda
"status"| "string"| Filtrar por estado
"order"| "string"| Orden de resultados

💡 Ejemplo

GET /catalogo/?page=1

📦 Respuesta JSON

{
  "ok": true,
  "pagina_actual": 1,
  "por_pagina": 24,
  "total_paginas": 100,
  "total_resultados": 2400,
  "resultados": [
    {
      "id": 123,
      "titulo": "Kimetsu no Yaiba",
      "sinopsis": "La historia sigue a Tanjiro Kamado...",
      "slug": "kimetsu-no-yaiba",
      "poster": "https://cdn.animeav1.com/img/media/poster/123.jpg",
      "url": "/anime/kimetsu-no-yaiba/"
    }
  ]
}

⚠️ Página fuera de rango

Si la página solicitada supera el número total de páginas:

{
  "ok": true,
  "pagina_actual": 999,
  "por_pagina": 24,
  "total_paginas": 100,
  "total_resultados": 2400,
  "resultados": [],
  "nota": "La página 999 está fuera de rango: el catálogo solo tiene 100 páginas con estos filtros."
}

---

<div align="center">🎌 AnimeAV1 API

Datos obtenidos de AnimeAV1 · API no oficial

</div>
