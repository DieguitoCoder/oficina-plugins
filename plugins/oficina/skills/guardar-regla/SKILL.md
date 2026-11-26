---
name: "guardar-regla"
description: "Convierte una corrección en una regla permanente en el manual del agente"
argument-hint: "nombre-del-agente + qué estuvo mal y cómo lo quieres"
disable-model-invocation: true
---

La regla de oro de la oficina: si un agente falla, casi siempre **falta algo en sus
instrucciones**. Vamos a arreglarlo en el manual, no solo en este chat.

Corrección del usuario: $ARGUMENTS

Haz esto:
1. Identifica de qué agente es (atlas / nova / forge / vera / iris).
2. Redacta la regla en **una o dos líneas, en inglés**, lista para su manual.
3. Dime si esa regla **choca** con alguna instrucción que ya tenga ese agente.
4. Agrégala al final de la sección `## Learned rules` de
   `.claude/agents/<agente>.md` (la más reciente abajo).
5. Confírmame en español qué regla guardaste y en qué agente.

## Plugin mode

Este plugin es de solo lectura (Claude Code lo reemplaza al actualizar): **no** escribas en la
carpeta del plugin. Si el repo actual tiene `.claude/agents/<agente>.md`, agrega la regla ahí.
Si no, muéstrame la regla lista para copiar y dime que la agregue a `## Learned rules` de
`.claude/agents/<agente>.md` en el repo de la oficina (así llega al plugin en la próxima versión).
