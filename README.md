<div align="center">

<img src="https://is.wuaze.com/static/icon/Icon.png" width="120" alt="AnimeAV1 Logo">

# AnimeAV1 API

### 🎌 Anime API · Jikan/MAL · SUB & DUB · JSON

[![API](https://img.shields.io/badge/API-Online-ff6b9d?style=for-the-badge)](https://www.mushoku.eu.cc/)
[![PHP](https://img.shields.io/badge/PHP-Native-777bb4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![License](https://img.shields.io/badge/License-Custom-ff9f43?style=for-the-badge)](#-licencia)

<br>

**AnimeAV1** es una API ligera de anime creada para proyectos, aplicaciones y sitios relacionados con anime.

[🌐 API](https://www.mushoku.eu.cc/) · [📚 Documentación](#-endpoints) · [🐛 Reportar problema](../../issues)

</div>

---

## ✨ Sobre AnimeAV1

AnimeAV1 proporciona información de anime en formato **JSON**, incluyendo información basada en **MyAnimeList/Jikan**, episodios, búsqueda, rankings y más.

Está diseñada para ser sencilla de integrar en aplicaciones web, aplicaciones móviles y otros proyectos relacionados con anime.

### 🌸 Características

- 🎌 Información de anime
- 🔎 Búsqueda por nombre
- 📺 Episodios
- 🎙️ SUB / DUB
- ⭐ Rankings
- 📅 Horarios
- 🔤 Búsqueda por letra
- 🆔 Información de MyAnimeList
- ⚡ Sistema de caché
- 🚦 Rate limit
- 📦 Respuestas JSON
- 🪶 Backend ligero

---

## 🌐 Servidores

### Servidor principal

https://www.mushoku.eu.cc/

### Servidor alternativo

https://ww2.mushoku.eu.cc/

> Servidor que conecta con AnimeAV1 CC solo SUB (ES) 

---

# 📚 Endpoints

Todos los endpoints devuelven información en formato **JSON** salvo cuando se indique lo contrario.

## 📦 Catálogo

GET /catalogo/

Obtiene el catálogo disponible de anime.

### Ejemplo

https://www.mushoku.eu.cc/catalogo/

---

## 🔎 Buscar anime

GET /buscar/?q={consulta}

Busca anime mediante una consulta.

### Ejemplo

https://www.mushoku.eu.cc/buscar/?q=Mushoku%20no%20Eiyuu

---

## 🎬 Información de anime

GET /anime/{slug}/

Obtiene información detallada de un anime.

### Ejemplo

https://www.mushoku.eu.cc/anime/mushoku-no-eiyuu-betsu-ni-skill-nanka-iranakatta-n-da-ga/

---

## ▶️ Episodio

GET /ep/{slug}/E{numero}/

Obtiene información correspondiente a un episodio.

### Ejemplo

https://www.mushoku.eu.cc/ep/mushoku-no-eiyuu-betsu-ni-skill-nanka-iranakatta-n-da-ga/E1/

---

## 🇯🇵 MyAnimeList

GET /mal/{slug}/

Obtiene información relacionada con MyAnimeList.

### Ejemplo

https://www.mushoku.eu.cc/mal/mushoku-no-eiyuu-betsu-ni-skill-nanka-iranakatta-n-da-ga/

---

## 🆕 Últimos lanzamientos

GET /ultimos/

Obtiene los últimos anime o episodios disponibles.

### Ejemplo

https://www.mushoku.eu.cc/ultimos/

---

## 🔥 Top anime

GET /top/

Obtiene el ranking de anime.

### Ejemplo

https://www.mushoku.eu.cc/top/

---

## 🔤 Anime por letra

GET /az/{letra}/

Obtiene anime que comienzan con una letra determinada.

### Ejemplo

https://www.mushoku.eu.cc/az/A/

---

## 📅 Horario

GET /horario/

Obtiene información del horario de emisión.

### Ejemplo

https://www.mushoku.eu.cc/horario/

---

# 📄 Formato de respuesta

AnimeAV1 utiliza **JSON** para las respuestas de la API.

Ejemplo conceptual:

{
  "title": "Mushoku no Eiyuu",
  "episodes": 12,
  "status": "Finished Airing"
}

La estructura exacta puede variar dependiendo del endpoint.

---

# 🚦 Rate Limit

30 solicitudes por minuto / IP

Si superas el límite, espera antes de realizar nuevas solicitudes.

---

# 🛠️ Tecnología

AnimeAV1 utiliza un backend ligero basado en:

- PHP nativo
- Apache
- .htaccess
- JSON
- Sistema de caché
- Jikan / MyAnimeList

No utiliza CakePHP ni FuelPHP.

---

# 📌 Política de uso

AnimeAV1 puede utilizarse gratuitamente para integrar información de anime en proyectos **sin fines de lucro**.

### ✅ Permitido

- Integrar la API en proyectos personales.
- Utilizarla en aplicaciones gratuitas.
- Utilizarla mediante tu propio dominio oficial.
- Crear interfaces que consuman AnimeAV1.

### ❌ No permitido

- Clonar AnimeAV1.
- Copiar o modificar el backend.
- Migrar el backend a otro servidor.
- Autohospedar una copia de la API.
- Redistribuir el código fuente.
- Revender la API.
- Utilizarla como servicio comercial sin autorización.
- Hacer pasar una copia modificada como AnimeAV1.

---

# 🧩 Atribución

Si utilizas AnimeAV1 en un proyecto, se recomienda mantener una referencia a:

AnimeAV1 API
https://www.mushoku.eu.cc/

No es necesario colocar publicidad.

---

# 🐛 Issues & abuso

Si encuentras:

- errores
- endpoints caídos
- respuestas incorrectas
- problemas de seguridad
- abuso del servicio

puedes abrir un **Issue** en este repositorio.

Por favor, evita realizar spam o solicitudes masivas que puedan afectar al servicio.

---

# 📜 Licencia

AnimeAV1 utiliza una **licencia personalizada**.

El acceso a la API puede utilizarse gratuitamente en proyectos no comerciales, pero el código y la infraestructura no pueden copiarse, modificarse, migrarse, clonarse, redistribuirse o alojarse por terceros sin autorización.

El uso comercial requiere autorización previa.

---

# 💗 Thanks for Visiting

<div align="center">

### Gracias por visitar AnimeAV1 ♡

<img src="https://count.getloli.com/@animeav1?name=animeav1&theme=flat&padding=7&offset=253&align=center&scale=1&pixelated=1" alt="AnimeAV1 visitor counter">

<br><br>

<img src="https://github-readme-utils.vercel.app/api/gif/anime" width="220" alt="Random anime waifu">

<br>

### またね！ ✨

</div>

---

<div align="center">

### 🎌 AnimeAV1

**Made with ❤️ for anime projects**

<img src="https://img.shields.io/badge/Anime-AV1-ff6b9d?style=flat-square">

<br><br>

⭐ If AnimeAV1 is useful for your project, consider giving this repository a star.

</div>
```0
