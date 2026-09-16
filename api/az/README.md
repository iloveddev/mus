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

# 🔤 Catálogo A-Z

Filtra el catálogo utilizando la letra inicial del título.

## 🔗 Endpoint

```http
GET /az/{letra}/
```

## ⚙️ Parámetros

| Parámetro | Tipo | Descripción |
|:---|:---:|:---|
| `{letra}` | `string` | Letra inicial |
| `page` | `int` | Página del catálogo |
| `order` | `string` | Orden de resultados |

## 💡 Ejemplo

```http
GET /az/a/
```

## 📦 Respuesta JSON

```json
{
  "ok": true,
  "letra": "A",
  "pagina_actual": 1,
  "por_pagina": 24,
  "total_paginas": 10,
  "total_resultados": 240,
  "resultados": [
    {
      "id": 123,
      "titulo": "Attack on Titan",
      "sinopsis": "Hace siglos, la humanidad fue masacrada...",
      "slug": "attack-on-titan",
      "poster": "https://cdn.animeav1.com/img/media/poster/123.jpg",
      "url": "/anime/attack-on-titan/"
    }
  ]
}
```

## 🔥 Orden popular

```http
GET /az/a/?order=popular
```

---

<p align="center">
  🔤 <strong>A → Z · Anime Catalog</strong>
</p>
