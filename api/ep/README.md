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

# ▶️ Episodio

Obtiene los servidores de reproducción y enlaces de descarga de un episodio.

## 🔗 Endpoint

```http
GET /ep/{slug}/E{numero}/
```

También puede utilizarse:

```http
GET /ep/{slug}/{numero}/
```

## 💡 Ejemplo

```http
GET /ep/kimetsu-no-yaiba/E1/
```

## 📦 Respuesta JSON

```json
{
  "ok": true,
  "anime": {
    "id": 123,
    "titulo": "Kimetsu no Yaiba",
    "slug": "kimetsu-no-yaiba"
  },
  "episodio": 1,
  "servers": {
    "DUB": [
      {
        "servidor": "Servidor 1",
        "url": "https://..."
      }
    ],
    "SUB": [
      {
        "servidor": "Servidor 1",
        "url": "https://..."
      }
    ]
  },
  "descargas": {
    "DUB": [
      {
        "servidor": "Servidor 1",
        "url": "https://..."
      }
    ],
    "SUB": [
      {
        "servidor": "Servidor 1",
        "url": "https://..."
      }
    ]
  }
}
```

## 🎧 Idiomas

| Código | Descripción |
|:---:|:---|
| `SUB` | Subtitulado |
| `DUB` | Doblaje |

---

<p align="center">
  ▶️ <strong>Streaming · SUB · DUB · Downloads</strong>
</p>
