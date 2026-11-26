# Plugin «oficina» para Claude Code

El equipo de la Oficina Agéntica dentro de tu propia sesión de Claude Code. El marketplace es
público: no necesitas cuenta de GitHub.

```text
/plugin marketplace add DieguitoCoder/oficina-plugins
/plugin install oficina@dieguitocoder
```

- **Agentes** `oficina:atlas`, `oficina:orion`, `oficina:clio`, … (los 14 del equipo).
  Pídeselos por nombre («usa oficina:nova para…») o con `@agent-oficina:nova`.
- **Rutinas**: `/oficina:nuevo-proyecto`, `/oficina:reporte-diario`, `/oficina:guardar-regla`,
  `/oficina:revision-semanal`.
- **Manual del equipo**: skill `oficina:manual` (se carga cuando hace falta).
- **Puente con la oficina**: skill `/oficina:oficina` y las herramientas MCP `oficina_estado`,
  `oficina_abrir`, `oficina_grafo` (pregunta al grafo de conocimiento del proyecto: código,
  documentación o todo) y `oficina_delegar`, que hablan con la app de escritorio abierta en este
  equipo (necesita `node` en el PATH).

Sin hooks, sin binarios y sin secretos: el plugin no ejecuta nada por su cuenta.

¿La oficina completa? Instala Node.js 22.13+ y ejecuta `npx @dieguitocoder/oficina@latest init`.

Este directorio lo genera `scripts/build-plugin.mjs` (repo privado `Agent-Office-Code`); no lo
edites a mano. Licencia: todos los derechos reservados.
