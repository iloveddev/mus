Top

- Endpoint Name: Top / Popularidad
- Método: "GET"
- Endpoint: "/top/"

Obtiene el catálogo ordenado por popularidad.

Parámetros

- "page" — Página del catálogo. Por defecto: "1".

Ejemplo

"GET /top/?page=1"

Respuesta JSON

{
  "ok": true,
  "pagina_actual": 1,
  "por_pagina": 0,
  "total_paginas": 0,
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
