# Currículum Interactivo & Asistente IA - Juan Álvarez Núñez

Este proyecto contiene una página web moderna, profesional y responsiva contenida en un único archivo (`index.html`) con CSS y JavaScript nativo integrado, optimizada para desplegarse directamente en **GitHub Pages**.

---

## 🚀 Características Principales

1. **Vídeo de Bienvenida en la Parte Superior Central (Avatar Interactivo):**
   - Placeholder en posición destacada arriba y al centro con reproducción automática (`autoplay muted playsinline loop`) y botón interactivo para activar audio.
   - Acompañado de la transcripción oficial del avatar:
     > *"¡Hola! Soy Juan Álvarez, graduado en International Business por ESIC y Grenoble École de Management, y actualmente estudiante de Data Science.*  
     > *Trabajo como analista de Inteligencia Artificial en Deloitte y tengo experiencia en proyectos de Data Science y consultoría tecnológica."*
   - Archivo esperado: `avatar.mp4` o `bienvenida.mp4`.

2. **Cabecera & Perfil Ejecutivo:**
   - Nombre: **Juan Álvarez Núñez**
   - Titular Profesional: *Artificial Intelligence Analyst I en Deloitte | Graduado en International Business | Estudiante de Data Science*
   - Enlaces de contacto directos: LinkedIn, GitHub, Email, Teléfono y Ubicación en Las Rozas de Madrid.

3. **Sección Multimedia con 3 Tarjetas de Vídeo:**
   - **Tarjeta 1 (`pitch.mp4`):** Presentación Ejecutiva | Elevator Pitch.
   - **Tarjeta 2 (`proyecto.mp4`):** Caso de Estudio | Demostración de Proyecto.
   - **Tarjeta 3 (`habilidades.mp4`):** Stack Técnico + Soft Skills | Habilidades Técnicas & Soft Skills (con énfasis en trayectoria internacional en España, Francia y Canadá, bilingüe en inglés y C1 de francés).
   - *Nota:* Se ha eliminado cualquier texto sobrante de metadata ("Archivo: ...").

4. **Asistente Virtual IA con Google Gemini:**
   - Conexión REST directa con los modelos `gemini-2.5-flash` y `gemini-1.5-flash` de Google AI Studio.
   - **System Instruction blindado:** Contiene de forma estructurada todo tu historial profesional (Deloitte, Webtools, h&k), proyectos reales, formación (ESIC, Grenoble École de Management), certificaciones (Azure, Python, SQL) y premios a la excelencia académica.
   - **Reglas de veracidad:** No inventa métricas ni proyectos no documentados en Deloitte y aclara tu situación laboral actual.

5. **Gestión Segura de API Key:**
   - El visitante introduce su propia clave de Google AI Studio.
   - Se guarda exclusivamente en el `localStorage` del navegador visitante. No se expone en el código fuente ni viaja a ningún servidor intermediario.

6. **Manejo Visual de Errores & Sugerencias:**
   - Chips interactivos con preguntas rápidas frecuentes.
   - Indicadores de mecanografía (*typing dots*).
   - Detección y presentación clara de errores (Clave inválida 400/403, Límite de cuota 429, fallos de conexión) con botón de reintento directo.

---

## 📁 Estructura de Archivos para Despliegue

```text
mi-cv-interactivo/
├── index.html          <-- Archivo principal con todo integrado
├── README.md           <-- Documentación para GitHub
└── videos/             <-- Carpeta con los vídeos locales
    ├── bienvenida.mp4  <-- Vídeo del avatar de bienvenida
    ├── pitch.mp4       <-- Vídeo de elevator pitch
    ├── proyecto.mp4    <-- Vídeo de demostración de proyecto
    └── habilidades.mp4 <-- Vídeo de habilidades técnicas + soft skills
```

---

## 🌐 Pasos para Desplegar en GitHub Pages

1. **Crear repositorio en GitHub:**
   - Ve a [GitHub](https://github.com/new) y crea un nuevo repositorio público (por ejemplo, `curriculum` o `juan-alvarez-cv`).

2. **Subir los archivos:**
   - Sube `index.html`, `README.md` y tus vídeos.
   - O mediante la terminal:
     ```bash
     git init
     git add index.html README.md avatar.mp4 pitch.mp4 proyecto.mp4 habilidades.mp4
     git commit -m "Deploy: Curriculum interactivo con avatar de bienvenida y Gemini AI"
     git branch -M main
     git remote add origin https://github.com/Juan446-pixel/TU-REPOSITORIO.git
     git push -u origin main
     ```

3. **Activar GitHub Pages:**
   - En tu repositorio de GitHub, dirígete a **Settings** > **Pages**.
   - En *Build and deployment > Source*, selecciona **Deploy from a branch**.
   - En *Branch*, selecciona `main` y la carpeta `/(root)`, luego pulsa **Save**.
   - ¡Listo! En un par de minutos tu web estará disponible en:
     `https://juan446-pixel.github.io/TU-REPOSITORIO/`
