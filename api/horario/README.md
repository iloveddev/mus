Horario

- Endpoint Name: Horario
- Método: "GET"
- Endpoint: "/horario/"

Obtiene los animes activos agrupados según el día real de publicación de su último episodio.

«AnimeAV1 no proporciona horarios fijos de emisión. Por ello, este endpoint utiliza la fecha de publicación del último episodio para determinar el día.»

Ejemplo

"GET /horario/"

Respuesta JSON

{
  "ok": true,
  "nota": "Agrupado por el día real de publicación del último episodio (AnimeAV1 no expone horarios fijos)",
  "horario": {
    "Domingo": [
      {
        "id": 0,
        "titulo": "...",
        "slug": "...",
        "tipo": "...",
        "poster": "https://cdn.animeav1.com/img/media/poster/0.jpg",
        "ultimo_episodio": 1,
        "publicado": "...",
        "url": "/anime/.../"
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
