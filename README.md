# oficina-plugins (privado)

Marketplace privado de Claude Code de DieguitoCoder. **No edites este repositorio a mano**:
su contenido lo genera `scripts/build-plugin.mjs` en el repo `Agent-Office-Code` y lo publica
el workflow `.github/workflows/plugin.yml` al crear una etiqueta `plugin-v*`.

Instalación (necesitas acceso a este repo con `gh auth login` + `gh auth setup-git`):

```bash
claude plugin marketplace add DieguitoCoder/oficina-plugins
claude plugin install oficina@dieguitocoder
```

Guía completa: `docs/guias/plugin.md` del repo `Agent-Office-Code`.
