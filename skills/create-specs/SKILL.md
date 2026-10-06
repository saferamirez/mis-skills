---
name: hacer-spec
description: "Convierte una idea en spec.md con recorridos y criterios testeables, sin stack ni código. Úsalo cuando el usuario pide especificar, escribir la spec o aclarar un feature. No lo uses para planear, partir tareas ni implementar."
type: workflow
lifecycle: active
---

# Hacer spec

Escribes solo `specs/NNN-nombre/spec.md`. No creas plan, tasks ni código.

## Entrada

Una frase o párrafo del usuario. Si no hay idea, para y pídela.

## Pasos

1. Crea `specs/NNN-nombre/` con el siguiente número libre. Nombre de 2 a 4 palabras.
2. Redacta el borrador con la plantilla de `references/plantilla-spec.md`. Qué y por qué. Prohibido nombrar framework, base de datos, API o archivo.
3. Marca con `[NECESITA CLARIFICACIÓN]` cada hueco que cambie el comportamiento: quién puede hacerlo, qué pasa si falla, límites de cantidad, qué queda fuera. Máximo cinco. Si hay más, la idea no está lista: dilo y para.
4. Haz las preguntas de una en una. Escribe cada respuesta dentro de la spec y borra el marcador. No acumules un cuestionario.
5. Completa el checklist del final. Un ítem sin marcar es un hueco, no un adorno.
6. Para. Entrega la ruta del archivo y espera aprobación. No sigas a plan ni a código aunque el usuario diga "y ahora hazlo" en el mismo mensaje.

## Listo cuando

- Cada recorrido tiene un criterio observable, no un adjetivo.
- Fuera de alcance nombra al menos una cosa que alguien pediría y no entra.
- Cero marcadores `[NECESITA CLARIFICACIÓN]`.
- Checklist completo.
