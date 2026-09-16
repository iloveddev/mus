Anime

- Endpoint Name: Información del Anime
- Método: "GET"
- Endpoint: "/anime/{slug}/"

Obtiene información del anime, géneros y lista de episodios.

Ejemplo

"GET /anime/kimetsu-no-yaiba/"

Respuesta JSON

{
  "ok": true,
  "id": 0,
  "titulo": "...",
  "sinopsis": "...",
  "slug": "kimetsu-no-yaiba",
  "poster": "https://cdn.animeav1.com/img/media/poster/0.jpg",
  "tipo": "...",
  "estado": 0,
  "año_inicio": "...",
  "año_fin": "...",
  "puntuacion": 0,
  "votos": 0,
  "total_episodios": 0,
  "generos": [
    {
      "nombre": "...",
      "slug": "..."
    }
  ],
  "episodios": [
    {
      "numero": 1,
      "url": "/ep/kimetsu-no-yaiba/E1/"
    }
  ],
  "mal": {
    "ok": true,
    "mal_id": 0,
    "titulo": "...",
    "puntuacion": 0,
    "ranking": 0,
    "estudios": [
      "..."
    ],
    "trailer": null,
    "url_mal": "..."
  }
}

El campo "mal" puede ser "null" si el anime no tiene información vinculada a MyAnimeList.
