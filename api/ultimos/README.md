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

# 🆕 Últimos

Obtiene los últimos episodios publicados y los animes agregados recientemente.

## 🔗 Endpoint

```http
GET /ultimos/
```

## 📦 Respuesta JSON

```json
{
  "ok": true,
  "ultimos_episodios": [
    {
      "anime": "Kimetsu no Yaiba",
      "slug": "kimetsu-no-yaiba",
      "episodio": 26,
      "publicado": "2019-09-28T10:00:00.000Z",
      "comentarios": 25,
      "url": "/ep/kimetsu-no-yaiba/E26/"
    }
  ],
  "animes_recientes": [
    {
      "id": 123,
      "titulo": "Kimetsu no Yaiba",
      "slug": "kimetsu-no-yaiba",
      "tipo": "TV",
      "agregado": "2026-09-16T10:00:00.000Z",
      "poster": "https://cdn.animeav1.com/img/media/poster/123.jpg",
      "url": "/anime/kimetsu-no-yaiba/"
    }
  ]
}
```

## 📌 Contenido

- `ultimos_episodios` — Episodios publicados recientemente.
- `animes_recientes` — Animes agregados recientemente.

---

<p align="center">
  🆕 <strong>Latest Episodes · New Anime</strong>
</p>
