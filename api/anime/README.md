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

# 🎬 Información del anime

Obtiene información detallada de un anime, sus géneros, episodios y datos de MyAnimeList.

## 🔗 Endpoint

```http
GET /anime/{slug}/
```

## 💡 Ejemplo

```http
GET /anime/kimetsu-no-yaiba/
```

## 📦 Respuesta JSON

```json
{
  "ok": true,
  "id": 123,
  "titulo": "Kimetsu no Yaiba",
  "sinopsis": "La historia sigue a Tanjiro Kamado...",
  "slug": "kimetsu-no-yaiba",
  "poster": "https://cdn.animeav1.com/img/media/poster/123.jpg",
  "tipo": "TV",
  "estado": 1,
  "año_inicio": "2019-04-06",
  "año_fin": "2019-09-28",
  "puntuacion": 8.5,
  "votos": 12345,
  "total_episodios": 26,
  "generos": [
    {
      "nombre": "Acción",
      "slug": "accion"
    },
    {
      "nombre": "Aventura",
      "slug": "aventura"
    }
  ],
  "episodios": [
    {
      "numero": 1,
      "url": "/ep/kimetsu-no-yaiba/E1/"
    },
    {
      "numero": 2,
      "url": "/ep/kimetsu-no-yaiba/E2/"
    }
  ],
  "mal": {
    "ok": true,
    "mal_id": 38000,
    "titulo": "Kimetsu no Yaiba",
    "puntuacion": 8.5,
    "ranking": 100,
    "estudios": [
      "ufotable"
    ],
    "trailer": "https://www.youtube.com/watch?v=...",
    "url_mal": "https://myanimelist.net/anime/38000/..."
  }
}
```

## 🍥 MyAnimeList

El campo `mal` contiene información adicional obtenida mediante Jikan/MyAnimeList cuando está disponible.

---

<p align="center">
  🎬 <strong>Anime Details · Episodes · MAL</strong>
</p>
