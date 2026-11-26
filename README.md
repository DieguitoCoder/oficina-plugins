# oficina-plugins

Marketplace **público** de Claude Code de DieguitoCoder: el equipo de agentes de la **Oficina
Agéntica** (14 agentes, el manual del equipo y las rutinas de la oficina) dentro de tu sesión de
Claude Code.

## Instalar

No necesitas cuenta de GitHub ni ningún permiso:

```bash
claude plugin marketplace add DieguitoCoder/oficina-plugins
claude plugin install oficina@dieguitocoder
```

Abre una sesión nueva de Claude Code y prueba `/oficina:nuevo-proyecto` o `@agent-oficina:nova`.

Actualizar: `claude plugin marketplace update dieguitocoder` y luego
`claude plugin update oficina@dieguitocoder`.

¿Error `Permission denied (publickey)`? Claude Code intentó usar SSH: pon la variable
`CLAUDE_CODE_PLUGIN_PREFER_HTTPS=1` (en PowerShell `setx CLAUDE_CODE_PLUGIN_PREFER_HTTPS 1`), abre
una terminal nueva y reintenta.

¿Quieres la oficina completa (servidor, oficina 3D, Telegram)? Instala Node.js 22.13+ y ejecuta
`npx @dieguitocoder/oficina@latest init`.

---

**No edites este repositorio a mano**: su contenido lo genera `scripts/build-plugin.mjs` en el repo
privado `Agent-Office-Code` y lo publica el workflow `.github/workflows/plugin.yml` al crear una
etiqueta `plugin-v*`. Licencia: todos los derechos reservados.
