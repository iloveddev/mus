Últimos

- Endpoint Name: Últimos episodios
- Método: "GET"
- Endpoint: "/ultimos/"

Obtiene los últimos episodios publicados y los animes agregados recientemente.

Ejemplo

"GET /ultimos/"

Respuesta JSON

{
  "ok": true,
  "ultimos_episodios": [
    {
      "anime": "...",
      "slug": "...",
      "episodio": 1,
      "publicado": "...",
      "comentarios": 0,
      "url": "/ep/.../E1/"
    }
  ],
  "animes_recientes": [
    {
      "id": 0,
      "titulo": "...",
      "slug": "...",
      "tipo": "...",
      "agregado": "...",
      "poster": "https://cdn.animeav1.com/img/media/poster/0.jpg",
      "url": "/anime/.../"
    }
  ]
}
