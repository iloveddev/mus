MyAnimeList

- Endpoint Name: Información de MyAnimeList
- Método: "GET"
- Endpoint: "/mal/{slug}/"

Obtiene información de MyAnimeList mediante Jikan.

Ejemplo

"GET /mal/kimetsu-no-yaiba/"

Respuesta JSON

`{
  "ok": true,
  "slug": "kimetsu-no-yaiba",
  "mal_id": 0,
  "titulo": "...",
  "titulo_ingles": "...",
  "titulo_japones": "...",
  "sinopsis": "...",
  "tipo": "...",
  "fuente": "...",
  "episodios": 0,
  "duracion": "...",
  "estado": "...",
  "emitido": "...",
  "temporada": "...",
  "año": 0,
  "puntuacion": 0,
  "ranking": 0,
  "popularidad": 0,
  "miembros": 0,
  "estudios": [
    "..."
  ],
  "productoras": [
    "..."
  ],
  "generos": [
    "..."
  ],
  "poster_mal": "...",
  "trailer": "...",
  "url_mal": "..."
}`
