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

1. Crea `specs/NNN-nombre/` con el siguiente número libre de tres dígitos. Nombre de 2 a 4 palabras.
2. Lee `references/plantilla-spec.md` y `references/ejemplo-spec.md` de este skill. Redacta el borrador con los títulos de la plantilla. Sustituye cada instrucción por contenido: en la spec no quedan las instrucciones. El ejemplo marca el nivel de concreción; no copies su tema. Desde el borrador cumple el ítem del checklist sobre nombres de tecnología.
3. Cada comportamiento sale de lo que el usuario dijo. Si un dato cambia el alcance, quién puede, qué pasa si falla o un límite de cantidad, márcalo en la sección correspondiente como `[NECESITA CLARIFICACIÓN: pregunta]`. Si no cambia el comportamiento, va en Supuestos. Máximo cinco marcadores, en este orden: alcance, quién puede, qué pasa si falla, límites de cantidad. Si hacen falta más de cinco, la idea no está lista: dilo y para. No conviertas un hueco de más en un supuesto.
4. Haz las preguntas de una en una. En cada una ofrece una respuesta recomendada y espera. Escribe la respuesta en la sección del marcador, anótala en Aclaraciones y borra el marcador.
5. Completa el checklist de la plantilla. Ese checklist es la definición de listo. Un ítem sin marcar es un hueco. No lo marques si el texto no lo cumple.
6. Para. Entrega la ruta del archivo y espera aprobación. No sigas a plan ni a código aunque el usuario diga "y ahora hazlo" en el mismo mensaje.
