# Simulador de Entrevista de Visa — para Cristina 🛂 🇺🇸

Juego interactivo para practicar la entrevista de visa americana de turista (B1/B2), basado en **preguntas reales** de entrevistas consulares.

## 🚀 Cómo subirlo a GitHub y compartirlo

1. Crea un repo nuevo en GitHub (ej: `practica-visa-cristina`). Que sea **público**.
2. Sube el archivo `index.html` (botón **Add file → Upload files**, arrastra el archivo, **Commit**).
3. Ve a **Settings → Pages** del repo.
4. En **Source** elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`. Guarda.
5. Espera 1–2 minutos. Aparecerá una URL (algo como `https://tuusuario.github.io/practica-visa-cristina/`).
6. Mándale ese link a Cristina por WhatsApp. Funciona en celular y computador, sin instalar nada.

> No necesita conexión a ninguna base de datos ni servidor: es un solo archivo que corre en el navegador.

## 🎮 Qué incluye

- **Paso 1 — Personalización (opcional):** Cristina mete sus datos reales (ciudad, trabajo, a quién visita, dónde se hospeda, fechas). Las "buenas respuestas" del juego usan **su historia real**.
- **Paso 2 — Vestimenta:** elige el outfit (con feedback).
- **Paso 3 — Documentos:** checklist de qué llevar a la entrevista (carta de invitación, estados de cuenta, carta laboral, vuelo ida y vuelta, etc.).
- **Entrevista en la ventanilla 7** con un oficial consular que:
  - Tiene un **medidor de confianza** en vivo (sube y baja según las respuestas).
  - **Cambia de cara y de humor** 🙂 → 😐 → 🤨 → 😠.
  - Suelta reacciones tipo *"Eso no me convence"* o *"Me queda claro"*.
- **32 preguntas reales** organizadas en 8 categorías. Cada partida mezcla un set distinto, priorizando las preguntas clave del caso de Cristina.
- **Dos modos** (puede cambiar en cualquier pregunta):
  - **Fácil:** escoge entre 3 respuestas; le explico por qué cada una es buena/regular/mala y le revelo la mejor.
  - **Difícil:** escribe su propia respuesta; la evalúo por palabras clave y banderas rojas, y le muestro una **respuesta modelo**.
- **Veredicto final:** VISA APROBADA / EN REVISIÓN / NEGADA, con sello visual, conteo de respuestas y **desglose por tema** (en qué categoría va bien y en cuál floja).
- **Atajos de teclado:** teclas `1` `2` `3` para elegir, `Enter` para avanzar.

## 🎯 Detalles pensados para el caso de Cristina

Caso precargado: **Cristina, de La Chorrera (Panamá)**, vive con su **abuela y su tía**, va al **Mundial 2026** y de paso a visitar a su **mamá** (que vive en EE.UU.).

- **El Mundial 2026 como motivo de viaje** — preguntas de "¿a qué partidos vas?" y "¿ya compraste las entradas?". Es un turismo claro y temporal (el Mundial termina → regresas), muy buen argumento.
- La pregunta de que **su mamá vive en EE.UU.** (la trampa de no mentir).
- El detalle de que **la mamá viajó antes y regresó** — con la respuesta ideal: convertirlo en un punto a favor ("mi familia respeta las reglas de la visa").
- **"¿No le tienta quedarse a vivir allá?"** — la pregunta trampa más importante de su situación.
- **Vivir con su abuela y tía en Panamá** como ancla fuerte (tiene un hogar al que volver).
- Quedarse en **casa de alguien conocido**, quién paga el viaje, vuelo de regreso, etc.

> ⚠️ Importante sobre la "excusa" del Mundial: funciona muy bien **solo si es real**. Cristina debe llevar **entradas compradas** (o al menos confirmaciones) y poder decir a qué partidos/ciudades va. Y aunque el Mundial sea el motivo principal, **no debe ocultar a la mamá** — si se lo preguntan, lo dice con naturalidad. Mentir es lo único que de verdad hunde una entrevista.

## 🗂️ Categorías de preguntas

Propósito del viaje · Duración/regreso · Alojamiento · Familia y vínculos · Finanzas · Lazos con tu país · Historial de viajes · Preguntas trampa.

## ✏️ Cómo editar el contenido

Todo está en un solo `index.html`. Las preguntas están en el array `QUESTIONS` (al inicio del `<script>`). Cada una tiene 3 opciones con su `rating` (`good`/`mid`/`bad`) y su feedback. Para agregar preguntas, copia el formato de una existente.

Los datos personalizables usan tokens como `{visita}`, `{ciudadUS}`, `{ocupacion}`, `{duracion}` — se rellenan solos con lo que Cristina escriba en el Paso 1 (o usan un texto neutral si lo deja en blanco).

## 📚 Fuentes de las preguntas

Las preguntas y los criterios de "buena/mala respuesta" se basaron en guías de entrevistas consulares B1/B2 (2025):
- Boundless — *B-1/B-2 Visa Sample Interview Questions*
- RumboVisa — *50 Preguntas Clave en la Entrevista de Visa Americana*
- Guías de preparación B1/B2 2025 (Atlys, Teleport, AfnoVisaGuide, inmigracionyvisas)

> Esto es material de práctica, no asesoría legal. Para casos con antecedentes o negaciones previas, conviene consultar a un abogado de inmigración.
