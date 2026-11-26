# Plugin «oficina» para Claude Code

El equipo de la Oficina Agéntica dentro de tu propia sesión de Claude Code.

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
  `oficina_abrir` y `oficina_delegar`, que hablan con la app de escritorio abierta en este
  equipo (necesita `node` en el PATH).

Sin hooks, sin binarios y sin secretos: el plugin no ejecuta nada por su cuenta.

Este directorio lo genera `scripts/build-plugin.mjs`; no lo edites a mano.
Guía: `docs/guias/plugin.md` del repo `Agent-Office-Code`.
