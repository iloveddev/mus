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

# 🍥 MyAnimeList

Obtiene información de MyAnimeList mediante Jikan.

## 🔗 Endpoint

```http
GET /mal/{slug}/
```

## 💡 Ejemplo

```http
GET /mal/kimetsu-no-yaiba/
```

## 📦 Respuesta JSON

```json
{
  "ok": true,
  "slug": "kimetsu-no-yaiba",
  "mal_id": 38000,
  "titulo": "Kimetsu no Yaiba",
  "titulo_ingles": "Demon Slayer: Kimetsu no Yaiba",
  "titulo_japones": "鬼滅の刃",
  "sinopsis": "Tanjiro Kamado, un joven vendedor de carbón...",
  "tipo": "TV",
  "fuente": "Manga",
  "episodios": 26,
  "duracion": "24 min",
  "estado": "Finished Airing",
  "emitido": "Apr 6, 2019 to Sep 28, 2019",
  "temporada": "Spring",
  "año": 2019,
  "puntuacion": 8.5,
  "ranking": 100,
  "popularidad": 50,
  "miembros": 2000000,
  "estudios": [
    "ufotable"
  ],
  "productoras": [
    "Aniplex",
    "Shueisha"
  ],
  "generos": [
    "Action",
    "Adventure",
    "Fantasy"
  ],
  "poster_mal": "https://cdn.myanimelist.net/images/anime/1286/99889l.jpg",
  "trailer": "https://www.youtube.com/watch?v=...",
  "url_mal": "https://myanimelist.net/anime/38000/Kimetsu_no_Yaiba"
}
```

## 🔌 Fuente

Los datos de este endpoint proceden de MyAnimeList mediante Jikan.

---

<p align="center">
  🍥 <strong>MyAnimeList · Jikan</strong>
</p>
