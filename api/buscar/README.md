Buscar

- Endpoint Name: Búsqueda
- Método: "GET"
- Endpoint: "/buscar/?q="

Busca animes por título.

Parámetros

- "q" — Término que se desea buscar. Obligatorio.
- "page" — Página de resultados. Por defecto: "1".

Ejemplo

"GET /buscar/?q=kimetsu"

Respuesta JSON

{
  "ok": true,
  "consulta": "kimetsu",
  "pagina_actual": 1,
  "total_resultados": 0,
  "resultados": [
    {
      "id": 0,
      "titulo": "...",
      "sinopsis": "...",
      "slug": "...",
      "poster": "https://cdn.animeav1.com/img/media/poster/0.jpg",
      "url": "/anime/..."
    }
  ]
}

Error

Si no se proporciona "q":

{
  "ok": false,
  "error": "Falta el parámetro ?q= con el término a buscar"
}
