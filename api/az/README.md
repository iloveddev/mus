A-Z

- Endpoint Name: Catálogo A-Z
- Método: "GET"
- Endpoint: "/az/{letra}/"

Obtiene los animes cuyo título comienza con la letra indicada.

Parámetros

- "{letra}" — Una letra de la A a la Z.
- "page" — Página del catálogo. Por defecto: "1".
- "order" — Orden opcional. Ejemplo: "popular".

Ejemplo

"GET /az/a/"

Respuesta JSON

{
  "ok": true,
  "letra": "A",
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
