# Barbería René

Web estática de una barbería con Astro, Tailwind CSS, GSAP, morphicons y scroll-world. Se despliega en Cloudflare Pages (`*.pages.dev`).

## Reglas obligatorias

- Usa SIEMPRE pnpm con preferencia offline: `pnpm add --prefer-offline` y `pnpm install --prefer-offline`. NUNCA uses npm, npx ni yarn; usa `pnpm dlx` o `pnpm create`.
- `--prefer-offline` puede resolver versiones antiguas desde la caché. Para cada dependencia, consulta antes la última versión con `pnpm view <paquete> version` e instala `<paquete>@<versión>`.
- NUNCA hagas push ni merge a `main`. La cuenta autenticada en gh es de colaborador y no es la dueña del repo, así que todo se sube desde una rama y por PR.
- Haz SIEMPRE un commit antes de cada cambio grande: scaffold, nuevas dependencias, cambios de configuración o refactors. Cada commit debe dejar el proyecto en un estado coherente.
- El despliegue es solo en Cloudflare. NO uses Vercel ni añadas configuración o dependencias suyas.

## Comandos

- Desarrollo: `pnpm dev`
- Build: `pnpm build` (genera `dist/`)
- Preview: `pnpm preview`

## scroll-world

`scroll-world` no es un paquete de npm, sino un skill para agentes (https://github.com/oso95/scroll-world). `src/vendor/scroll-world/` contiene una copia sin modificar de su motor, con su licencia MIT. Generar los vídeos de las escenas tiene coste, así que hay que pedir aprobación antes.
