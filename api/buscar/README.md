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

# 🔎 Buscar anime

Busca animes por título.

## 🔗 Endpoint

```http
GET /buscar/?q=
```

## ⚙️ Parámetros

| Parámetro | Tipo | Requerido | Descripción |
|:---|:---:|:---:|:---|
| `q` | `string` | ✅ | Término de búsqueda |
| `page` | `int` | ❌ | Página de resultados |

## 💡 Ejemplo

```http
GET /buscar/?q=kimetsu
```

## 📦 Respuesta JSON

```json
{
  "ok": true,
  "consulta": "kimetsu",
  "pagina_actual": 1,
  "total_resultados": 1,
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

## ❌ Falta `q`

```json
{
  "ok": false,
  "error": "Falta el parámetro ?q= con el término a buscar"
}
```

---

<p align="center">
  🔎 <strong>Busca · Encuentra · Consume</strong>
</p>
