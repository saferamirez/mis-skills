# Spec: <nombre>

## Problema

Quién sufre qué, y por qué importa ahora. Máximo tres líneas.

## Usuario

El actor de esta fase. Si hay más de uno, di cuál no entra todavía.

## Cosas

Para cada cosa: cómo se reconoce, qué datos ve el usuario, cuáles son obligatorios y cuáles puede cambiar. Si no hay datos, escribe "Sin cosas que guardar".

## Estados

Si la cosa cambia de situación, lista los estados y quién pasa de uno a otro. Si no hay ciclo de vida, escribe "Sin estados".

## Recorridos

1. <nombre>
   - Empieza: <estado inicial>
   - Hace: <acción>
   - Termina: <resultado que una persona comprueba mirando qué quedó>
   - Sigue igual: <qué no cambia>
   - Si falla: <dato inválido, no existe, sin permiso o ya estaba hecho>. Si no puede fallar, escribe "No falla".

## Criterios de aceptación

Un criterio por recorrido y uno por cada fallo:

- Dado <estado>, cuando <acción>, entonces <resultado comprobable>.

## Fuera de alcance

Al menos una cosa que el texto sugiere, que alguien pediría, y que no entra en esta fase.

## Supuestos

Lo que no cambia el comportamiento y se asume para seguir. Un supuesto no es un criterio de aceptación. Si no hay, escribe "Ninguno".

## Aclaraciones

- Pregunta → respuesta.

## Checklist

- [ ] Cada comportamiento viene de lo que el usuario dijo o de una respuesta en Aclaraciones
- [ ] Cosas y Estados están escritos, aunque sea para decir que no aplican
- [ ] Cada recorrido tiene empieza, hace, termina y sigue igual
- [ ] Cada entonces se comprueba mirando el resultado
- [ ] Cada recorrido tiene su fallo, o dice "No falla"
- [ ] Fuera de alcance nombra al menos una cosa que alguien pediría
- [ ] Ningún supuesto aparece como criterio
- [ ] Cero marcadores `[NECESITA CLARIFICACIÓN]`
- [ ] No hay nombres de framework, base de datos, API ni archivo
