Catálogo

- Endpoint Name: Catálogo
- Método: "GET"
- Endpoint: "/catalogo/"

Obtiene una lista de animes del catálogo.

Parámetros opcionales

- "page" — Página del catálogo. Por defecto: "1".
- "genre" — Filtra por género.
- "search" — Filtra por búsqueda.
- "status" — Filtra por estado.
- "order" — Orden de resultados. Ejemplo: "popular".

Ejemplo

"GET /catalogo/?page=1"

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

Si se solicita una página fuera del rango disponible:

{
  "ok": true,
  "pagina_actual": 999,
  "por_pagina": 0,
  "total_paginas": 0,
  "total_resultados": 0,
  "resultados": [],
  "nota": "La página 999 está fuera de rango: el catálogo solo tiene 0 páginas con estos filtros."
}
