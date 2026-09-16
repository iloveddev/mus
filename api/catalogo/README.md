<p align="center">
  <img src="https://is.wuaze.com/static/icon/Icon.png" width="120" alt="AnimeAV1 Logo">
</p>

<h1 align="center">AnimeAV1 API</h1>

<p align="center">
  🎌 Anime API · Jikan/MAL · SUB & DUB · JSON
</p>

<p align="center">
  <a href="https://www.mushoku.eu.cc/">
    <img src="https://img.shields.io/badge/API-Online-ff6b9d?style=for-the-badge" alt="API Online">
  </a>
  <a href="https://www.php.net/">
    <img src="https://img.shields.io/badge/PHP-Native-777bb4?style=for-the-badge&logo=php&logoColor=white" alt="PHP Native">
  </a>
  <img src="https://img.shields.io/badge/License-Custom-ff9f43?style=for-the-badge" alt="Custom License">
</p>

<p align="center">
  <strong>AnimeAV1</strong> es una API ligera de anime creada para proyectos, aplicaciones y sitios relacionados con anime.
</p>

<p align="center">
  <a href="https://www.mushoku.eu.cc/">🌐 API</a> ·
  <a href="#-endpoint">📚 Documentación</a> ·
  <a href="../../issues">🐛 Reportar problema</a>
</p>

---

# 📚 Catálogo

Obtiene los animes disponibles en el catálogo de AnimeAV1.

## 🔗 Endpoint

```http
GET /catalogo/
```

## ⚙️ Parámetros

| Parámetro | Tipo | Descripción |
|:---|:---:|:---|
| `page` | `int` | Página del catálogo |
| `genre` | `string` | Filtrar por género |
| `search` | `string` | Filtrar por búsqueda |
| `status` | `string` | Filtrar por estado |
| `order` | `string` | Orden de resultados |

## 💡 Ejemplo

```http
GET /catalogo/?page=1
```

## 📦 Respuesta JSON

```json
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
```

## ⚠️ Página fuera de rango

```json
{
  "ok": true,
  "pagina_actual": 999,
  "por_pagina": 24,
  "total_paginas": 100,
  "total_resultados": 2400,
  "resultados": [],
  "nota": "La página 999 está fuera de rango: el catálogo solo tiene 100 páginas con estos filtros."
}
```

---

<p align="center">
  🎌 <strong>AnimeAV1 API</strong><br>
  <sub>Datos obtenidos de AnimeAV1 · API no oficial</sub>
</p>
