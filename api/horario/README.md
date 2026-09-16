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

# 📅 Horario

Obtiene los animes activos agrupados por el día real de publicación de su último episodio.

## 🔗 Endpoint

```http
GET /horario/
```

## ℹ️ Información

AnimeAV1 no expone horarios fijos de emisión.

Este endpoint utiliza la fecha de publicación del último episodio para determinar el día de la semana correspondiente.

## 📦 Respuesta JSON

```json
{
  "ok": true,
  "nota": "Agrupado por el día real de publicación del último episodio (AnimeAV1 no expone horarios fijos)",
  "horario": {
    "Domingo": [
      {
        "id": 123,
        "titulo": "Kimetsu no Yaiba",
        "slug": "kimetsu-no-yaiba",
        "tipo": "TV",
        "poster": "https://cdn.animeav1.com/img/media/poster/123.jpg",
        "ultimo_episodio": 26,
        "publicado": "2019-09-28T10:00:00.000Z",
        "url": "/anime/kimetsu-no-yaiba/"
      }
    ],
    "Lunes": [],
    "Martes": [],
    "Miércoles": [],
    "Jueves": [],
    "Viernes": [],
    "Sábado": []
  }
}
```

## 📆 Días disponibles

```text
Domingo
Lunes
Martes
Miércoles
Jueves
Viernes
Sábado
```

---

<p align="center">
  📅 <strong>Anime Schedule · Latest Episode</strong>
</p>
