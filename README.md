# mus
AnimeAV1 API

API no oficial para acceder de forma estructurada a información del catálogo de AnimeAV1, episodios, servidores de reproducción, descargas y datos adicionales de MyAnimeList.

«🚧 Proyecto en desarrollo: esta API puede recibir cambios y nuevos endpoints.»

🌐 Servidores

Servidor principal

https://www.mushoku.eu.cc/

Servidor alterno — próximamente

http://ww2.mushoku.eu.cc/

El servidor "ww2" será habilitado próximamente como servidor alternativo, pensado para ofrecer otra ruta de acceso a la API cuando el servidor principal no esté disponible o presente problemas de carga.

---

🚀 Endpoints

📚 Catálogo

GET /catalogo/

Obtiene el catálogo de AnimeAV1.

Parámetros opcionales:

?page=1
&genre=accion
&search=kimetsu
&status=
&order=popular

Ejemplo:

/catalogo/?page=1

---

🔎 Buscar anime

GET /buscar/?q=

Realiza una búsqueda dedicada por título.

Ejemplo:

/buscar/?q=kimetsu

También permite paginación:

/buscar/?q=kimetsu&page=2

---

🎬 Información de un anime

GET /anime/{slug}/

Devuelve información del anime y su lista de episodios.

Ejemplo:

/anime/kimetsu-no-yaiba/

---

▶️ Episodio

GET /ep/{slug}/E{numero}/

Obtiene los servidores de reproducción disponibles, separados por idioma, además de los enlaces de descarga disponibles.

Ejemplo:

/ep/kimetsu-no-yaiba/E1/

La respuesta puede incluir:

{
  "servers": {
    "DUB": [],
    "SUB": []
  },
  "descargas": {
    "DUB": [],
    "SUB": []
  }
}

---

⭐ MyAnimeList

GET /mal/{slug}/

Obtiene información adicional de MyAnimeList mediante Jikan, incluyendo:

- Título
- Título japonés
- Título inglés
- Sinopsis
- Tipo
- Episodios
- Estado
- Temporada
- Año
- Puntuación
- Ranking
- Popularidad
- Estudios
- Productoras
- Géneros
- Poster
- Trailer
- URL de MyAnimeList

Ejemplo:

/mal/kimetsu-no-yaiba/

---

🆕 Últimos

GET /ultimos/

Devuelve:

- Últimos episodios publicados
- Animes agregados recientemente
- Información básica de cada anime

---

🔥 Top

GET /top/

Obtiene el catálogo ordenado por popularidad.

También permite paginación:

/top/?page=2

---

🔤 A-Z

GET /az/{letra}/

Filtra el catálogo utilizando la primera letra del anime.

Ejemplo:

/az/a/

También acepta paginación:

/az/a/?page=2

Y ordenamiento:

/az/a/?order=popular

---

📅 Horario

GET /horario/

Obtiene los animes actualmente en emisión, agrupados según el día correspondiente a su último episodio.

---

⚡ Ejemplos completos

Con el servidor principal:

https://www.mushoku.eu.cc/catalogo/?page=1

https://www.mushoku.eu.cc/buscar/?q=kimetsu

https://www.mushoku.eu.cc/anime/kimetsu-no-yaiba/

https://www.mushoku.eu.cc/ep/kimetsu-no-yaiba/E1/

https://www.mushoku.eu.cc/mal/kimetsu-no-yaiba/

https://www.mushoku.eu.cc/ultimos/

https://www.mushoku.eu.cc/top/

https://www.mushoku.eu.cc/az/a/

https://www.mushoku.eu.cc/horario/

---

🛡️ Rate Limit

La API incorpora un límite de:

30 solicitudes por minuto / IP

Si se supera el límite, la API responde con:

429 Too Many Requests

---

🧩 Respuesta de la API

Las respuestas exitosas utilizan:

{
  "ok": true
}

Los errores utilizan códigos HTTP apropiados, por ejemplo:

400 — Parámetros incorrectos
404 — Recurso no encontrado
429 — Demasiadas solicitudes
502 — Error al obtener/procesar datos externos
500 — Error interno

---

📦 Características

- REST API
- Respuestas JSON
- Búsqueda de anime
- Catálogo paginado
- Filtro A-Z
- Orden por popularidad
- Últimos episodios
- Horario de emisión
- Información de episodios
- Servidores DUB/SUB
- Enlaces de descarga
- Información de MyAnimeList mediante Jikan
- Cache para reducir solicitudes externas
- Rate limiting por IP
- Servidor alterno en preparación

---

⚠️ Aviso

Esta es una API no oficial y no está afiliada oficialmente con AnimeAV1, MyAnimeList ni Jikan.

La API funciona como una capa de acceso estructurado a información obtenida desde servicios externos.

Los datos, disponibilidad de servidores y estructura de las fuentes externas pueden cambiar sin previo aviso.

---

📄 Licencia

Consulta el archivo "LICENSE" de este repositorio para conocer los términos de uso del proyecto.

---

🌐 Estado de servidores

Servidor| Estado
"www.mushoku.eu.cc"| 🟢 Principal
"ww2.mushoku.eu.cc"| 🟡 Próximamente

AnimeAV1 API — una API simple, rápida y estructurada para tus proyectos.
