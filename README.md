# Horus Prosthetics — Newsletter

Este paquete tiene todo lo necesario para editar y enviar el newsletter mensual de Horus Prosthetics, ya con la identidad de marca aplicada (paleta Black / White / Blue Jeans, logo oficial, tipografía con respaldo web-safe).

## ⚠️ Antes de enviar — 2 pendientes de esta edición

1. **Historia de Karla Rojas**: no encontré información pública sobre ella, así que el bloque "Historias que caminan" quedó marcado como `PENDIENTE DE CONTENIDO` en el HTML (verás una caja punteada azul). Necesito que me compartas: su historia (cómo empezó en el para-ciclismo, logros, un obstáculo que superó), una cita textual suya, una foto, y confirmación de que autorizó publicar su nombre y foto.
2. **Logo**: la URL usada (`horus-logo-white-full.png`) es la que carga en horusleg.com, pero un chequeo automático recibió un 403 (probable protección anti-bot del CDN ante peticiones que no vienen de un navegador real). **Abre `index.html` con Live Server o el archivo directamente en tu navegador para confirmar que el logo se ve.** Si no carga, descarga el PNG desde el sitio y súbelo a la librería de imágenes de Mailchimp/Brevo, luego reemplaza el `src` por esa nueva URL.

## Archivos

- **`index.html`** — la plantilla del correo, lista para editar. Todo el CSS está en línea a propósito (así lo exigen los clientes de correo).
- **`GUIA-ESTRATEGIA-NEWSLETTER.md`** — la guía de estrategia: frecuencia, estructura, tono, herramientas de envío y checklist antes de cada envío.

## Identidad de marca aplicada

- **Colores**: fondo negro `#000000` (prioridad 1), blanco `#FFFFFF` (prioridad 2) para textos, y Blue Jeans `#3EA2FF` (prioridad 3) como acento en etiquetas de sección, links y el bloque "¿Sabías que...?".
- **Tipografía**: los títulos usan una familia de respaldo tipo *Arial Black / Impact* en mayúsculas para aproximar Lemon Milk, y el cuerpo usa *Century Gothic / Futura* como respaldo de Geometria. Los clientes de correo (especialmente Outlook de escritorio) no cargan fuentes personalizadas de forma confiable, por eso no se puede insertar la fuente real Lemon Milk/Geometria vía `@font-face` sin arriesgar que se vea inconsistente. Si consigues los archivos web (`.woff`/`.woff2`) con licencia de uso, puedo añadir `@font-face` como mejora progresiva para los clientes que sí lo soportan (Apple Mail, Gmail en iOS/Android).
- **Botones**: sólido en Blue Jeans para la acción principal (coherente con tu botón de marca), y con borde blanco para acciones secundarias — mayúsculas y negrita, como indican tus guidelines para subheadings/botones.

## Cómo editarlo en VS Code

1. Abre esta carpeta en VS Code (`Archivo → Abrir carpeta...`).
2. Abre `index.html`. Busca la palabra `EDITAR` dentro de los comentarios del código — cada uno marca un texto, fecha, enlace o imagen que debes actualizar antes de enviar.
3. Instala la extensión **Live Server** (de Ritwick Dey) si quieres ver una vista previa en el navegador mientras editas: clic derecho sobre `index.html` → "Open with Live Server".
4. Reemplaza cada `src="https://placehold.co/..."` por la URL pública de tu foto real. Súbela primero a tu sitio web, a Cloudinary, Imgur o directamente a tu plataforma de envío — los correos no pueden cargar imágenes desde tu computadora.

## Cómo enviarlo

1. Copia todo el contenido de `index.html`.
2. En Mailchimp o Brevo, crea una campaña nueva y busca la opción **"Importar código HTML"** o **"Pegar código"** (no "diseñar desde cero").
3. Pega el código.
4. Verifica que las imágenes se vean (si usaste rutas locales, reemplázalas primero).
5. Envía una prueba a tu propio correo y revísala en el celular antes del envío masivo.

El paso a paso completo, con la lógica detrás de cada sección, está en `GUIA-ESTRATEGIA-NEWSLETTER.md`.

## Contenido de esta edición

- **Innovación Horus**: misión y precios reales de Horus Prosthetics (fuente: horusleg.com, businessempresarial.com.pe). Sigue siendo el mismo contenido de ejemplo — dime si quieres mostrar un producto específico (rodilla, pie protésico, etc.) esta vez.
- **Historias que caminan**: Karla Rojas, para-atleta de ciclismo — **pendiente de contenido real**, ver arriba.
- **Comunidad en movimiento**: 16 de octubre, Día Nacional de la Persona con Discapacidad en el Perú (fuente: observatorio.conadisperu.gob.pe). Es una fecha nacional confirmada y recurrente; la actividad local específica (municipalidad, feria, campaña) queda como "por confirmar" — complétala en cuanto la tengan.

Todo esto es reemplazable — la idea es que veas el formato funcionando con datos reales, no que uses este contenido literal cada mes.
