# Flujo de trabajo con Git y GitHub

## Ramas

- `main`: versión revisada de la documentación. No se escribe directamente sobre ella después del commit inicial.
- `docs/<tema>`: una rama por cada pieza de documentación (por ejemplo, `docs/bpmn-proceso-comercial`).

Cada rama se integra a `main` mediante un Pull Request.

## Mensajes de commit

Se usa la convención *Conventional Commits*, con la descripción en español y en modo imperativo:

```
<tipo>(<alcance opcional>): <descripción breve>
```

| Tipo | Uso |
|------|-----|
| `docs` | Documentación nueva o modificada. |
| `fix` | Corrección de un error en un documento o diagrama. |
| `chore` | Tareas de mantenimiento del repositorio. |

Ejemplos: `docs(bpmn): modelar el proceso comercial con CRM`, `fix(bpmn): corregir la etiqueta de la compuerta de seguimiento`.

## Pull Requests y revisión

- Cada Pull Request usa la plantilla de [`.github/pull_request_template.md`](../.github/pull_request_template.md), que incluye una lista de control de revisión.
- El PR referencia los *issues* del tablero que afecta (`Refs #n`).
- Se integra con *merge commit* para conservar en `main` el historial de cada rama.

### Revisión en un trabajo individual

El trabajo práctico es individual, por lo que no hay un par que revise. GitHub no permite que el autor apruebe su propio Pull Request, de modo que la revisión se realiza como **autorrevisión formal**: el autor recorre la lista de control, deja comentarios de revisión en el PR y, si encuentra observaciones, las corrige con commits adicionales antes de integrar. El historial de cada PR conserva esa evidencia.
