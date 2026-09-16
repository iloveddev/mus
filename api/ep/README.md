Episodio

- Endpoint Name: Episodio
- Método: "GET"
- Endpoint: "/ep/{slug}/E{numero}/"

Obtiene los servidores de streaming y enlaces de descarga de un episodio.

También acepta el número sin "E", por ejemplo "/ep/kimetsu-no-yaiba/1/".

Ejemplo

"GET /ep/kimetsu-no-yaiba/E1/"

Respuesta JSON

{
  "ok": true,
  "anime": {
    "id": 0,
    "titulo": "...",
    "slug": "kimetsu-no-yaiba"
  },
  "episodio": 1,
  "servers": {
    "DUB": [
      {
        "servidor": "...",
        "url": "..."
      }
    ],
    "SUB": [
      {
        "servidor": "...",
        "url": "..."
      }
    ]
  },
  "descargas": {
    "DUB": [
      {
        "servidor": "...",
        "url": "..."
      }
    ],
    "SUB": [
      {
        "servidor": "...",
        "url": "..."
      }
    ]
  }
}

"DUB" y "SUB" solamente aparecen cuando existen servidores para ese idioma.
