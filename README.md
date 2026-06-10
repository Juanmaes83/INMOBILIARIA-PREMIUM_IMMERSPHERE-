# IMMERSPHERE — Villa Siena · Bel Air
**Luxury Real Estate Digital Experience · RUBIK SOTA**

Landing one-page nivel Awwwards para Villa Siena (607 Siena Way, Bel Air, CA 90077).
Estética: documental de arquitectura + editorial de lujo. Dark mode, bronce champán,
Cormorant Garamond + Archivo, GSAP/ScrollTrigger.

## Estructura
```
index.html        → Web completa, autocontenida (HTML+CSS+JS, sin build)
PROMPT_MASTER.md  → Prompt maestro v2 reutilizable para futuras propiedades
README.md
```

## Ver en local
Doble clic en `index.html` o:
```bash
python3 -m http.server 8080
# → http://localhost:8080
```

## Subir a GitHub (tu repo)
```bash
git remote add origin https://github.com/Juanmaes83/INMOBILIARIA-PREMIUM_IMMERSPHERE-.git
git branch -M main
git push -u origin main
```
GitHub te pedirá usuario + Personal Access Token (Settings → Developer settings →
Fine-grained tokens → permiso "Contents: write" solo para este repo).

## Publicar con GitHub Pages
Repo → Settings → Pages → Source: `main` / root → Save.
URL resultante: `https://juanmaes83.github.io/INMOBILIARIA-PREMIUM_IMMERSPHERE-/`

## Datos de la propiedad (verificados 10/06/2026)
| Dato | Valor | Fuente |
|---|---|---|
| Precio actual | $135.000.000 | Redfin · MLS# 25627803 (relisting) |
| Precio anterior | $177.000.000 | MLS# 25497697 |
| Interior | 35.000 sq ft + rooftop 12.000 sq ft | MLS |
| Suites / Baños | 8 / 25 (10 completos + 15 aseos) | MLS |
| Parcela / Plantas | 1,22 acres / 4 | MLS |
| Arquitecto | Ardie Tavangarian — Arya Group | Listing |

## Supuestos declarados
- **Imágenes**: stock representativo (Unsplash License) con disclaimer en footer.
  Las fotos del listing tienen copyright del MLS/fotógrafo y no pueden usarse sin
  licencia. Swap directo cuando haya assets licenciados.
- **Vídeos**: los 4 slots del Cinematic Tour están preparados (`data-video`) para
  recibir los clips image-to-video de la Fase 2 (Higgsfield/Kling/Veo).
- **Formulario**: confirmación front-end; conexión a Supabase/email en Fase 5.

## Roadmap
F2 Vídeos cinematográficos · F3 Master film + voiceover · F4 Brochure/Social ·
F5 Backend formulario + GA4.

---
Demo project · Property data believed reliable but not guaranteed · Equal Housing Opportunity.
