# PROMPT MAESTRO v2 — IMMERSPHERE LUXURY ESTATE EXPERIENCE
**RUBIK SOTA · Plantilla reutilizable por propiedad · v10/06/2026**

> Por qué v2: el prompt v1 era una wishlist de 15 entregables sin orden de ejecución,
> sin validación de datos, sin estrategia legal de imágenes y con specs imposibles de
> verificar ("ARRI Alexa 35"). v2 separa CONTEXTO / DATOS / DISEÑO / EJECUCIÓN / QA,
> es ejecutable por fases y cada fase tiene criterio de aceptación.

---

## BLOQUE 0 — ROL Y RESULTADO

Actúa como dirección creativa + lead developer de un estudio digital ganador de
Awwwards especializado en real estate ultra-premium (referencias: Sotheby's,
The Agency, Aman, Apple, AD). Resultado de esta fase: **una landing one-page
production-ready** que se sienta como un documental de arquitectura, no como
un portal inmobiliario. Una sola fase por conversación. No avances de fase sin
mi OK.

## BLOQUE 1 — DATOS (fuente de verdad)

- Propiedad: [DIRECCIÓN + URL del listing]
- **Verifica los datos con búsqueda web ANTES de escribir una sola línea.**
  Contrasta mínimo 3 fuentes (MLS/Redfin/broker). Si hay discrepancia
  (precio, baños, m²), usa la fuente más reciente y decláralo.
- Entrega primero un **Property Intelligence Report** (tabla: dato / valor /
  fuente / fecha) y espera mi validación.
- PROHIBIDO: inventar datos, scrapear fotos del MLS (copyright). Imágenes:
  [A] assets licenciados que yo suba, o [B] stock representativo (Unsplash)
  con disclaimer visible en footer. Indica cuál usas.

## BLOQUE 2 — DIRECCIÓN DE ARTE (tokens, no adjetivos)

- Mood: arquitectura editorial, quiet wealth, cine documental.
- Paleta (declárala en CSS vars): negro cálido ~#0B0907, marfil ~#ECE5D8,
  bronce champán ~#B6995C, piedra ~#92886F. Un solo acento. Nada de morados.
- Tipografía: display serif con carácter (Cormorant Garamond u otra que
  justifiques) + sans no-genérica para cuerpo/UI (NO Inter, NO Roboto).
- Whitespace extremo. Sin gradientes decorativos, sin glassmorphism genérico,
  sin emojis, sin estética IA.
- **Elemento firma obligatorio**: propone 1 elemento memorable único derivado
  de la propiedad (ej.: rail de timecodes documental, corte de sección por
  plantas) y justifícalo en 2 líneas antes de construir.

## BLOQUE 3 — ARQUITECTURA DE LA PÁGINA (10 capítulos)

01 Hero cinematográfico (letterbox, video-ready con fallback imagen, nombre,
   ubicación, arquitecto, precio, CTA "Private Showing")
02 Manifesto (storytelling: por qué existe esta casa)
03 Visión arquitectónica (arquitecto, filosofía, materiales)
04 Lifestyle por capítulos editoriales (living, wellness, cine, colección…)
05 Floorplan/corte de sección interactivo (hover/click por niveles)
06 Cinematic tour (4 slots de vídeo con lightbox, posters mientras no haya vídeo)
07 Galería curada (12 imágenes, masonry museístico, captions)
08 Location intelligence (distancias reales, aviación privada, sin mapa fake)
09 Datos de la finca (grid editorial, no estilo MLS)
10 Private showing (formulario concierge: nombre, email, rol, mensaje;
    validación front; preparado para conectar a Supabase/email)

## BLOQUE 4 — STACK Y EJECUCIÓN

- **Un solo index.html autocontenido** (HTML+CSS+JS vanilla + GSAP/ScrollTrigger
  por CDN). Cero build. Desplegable en GitHub Pages tal cual.
- Motion: intro orquestada (1 momento), reveals on-scroll, parallax sutil,
  60fps, `prefers-reduced-motion` respetado. Nada de efectos de plantilla.
- Responsive real hasta 360px. Lazy-loading en todas las imágenes salvo hero.

## BLOQUE 5 — SEO + LEGAL (no negociable)

- Title <60c, meta description <160c, OG + Twitter Cards.
- JSON-LD schema.org `SingleFamilyResidence`.
- Alt text descriptivo en todas las imágenes.
- Footer: disclaimer de datos ("believed reliable but not guaranteed"),
  origen de imágenes, Equal Housing Opportunity, autoría del estudio.

## BLOQUE 6 — QA ANTES DE ENTREGAR

- [ ] Todos los datos coinciden con el Intelligence Report
- [ ] Todas las URLs de imagen devuelven 200 (verifícalo, no lo asumas)
- [ ] Sin scroll horizontal en móvil
- [ ] Formulario valida y confirma
- [ ] Lighthouse mental: LCP <2.5s (hero con fetchpriority, resto lazy)
- [ ] El diseño NO podría confundirse con una plantilla

## FASES POSTERIORES (conversaciones separadas, bajo demanda)

F2 · 4 vídeos cinematográficos image-to-video (Higgsfield/Kling/Veo: fidelidad
    total a la imagen fuente, movimiento sutil, 4s, sin morphing) → swap en hero
    y lightbox. F3 · Master film 25s + voiceover (perfil: narrador 45a, documental,
    sin lenguaje de agente). F4 · Brochure PDF + Reels/Shorts + email assets.
    F5 · Backend formulario (Supabase + RLS) y analítica GA4.
