# Spec: cancelar reserva

## Problema

Quien reservó una mesa no puede liberarla si ya no va a ir. La mesa queda ocupada y el local no puede ofrecerla.

## Usuario

La persona que hizo la reserva. El personal del local no entra en esta fase.

## Cosas

- Reserva. Se reconoce por el día, la hora y el nombre de quien reservó. Ve día, hora, cantidad de personas y estado. Obligatorios: día, hora y cantidad. En este recorrido solo puede cambiar el estado a Cancelada.

## Estados

- Confirmada → Cancelada. Solo quien hizo la reserva.
- Cancelada no pasa a otro estado.

## Recorridos

1. Cancelar una reserva confirmada
   - Empieza: tiene una reserva Confirmada en un día posterior a hoy
   - Hace: elige esa reserva y confirma la cancelación
   - Termina: la reserva queda Cancelada y ya no aparece entre las de día posterior a hoy
   - Sigue igual: día, hora, cantidad y nombre
   - Si falla: ya estaba Cancelada

## Criterios de aceptación

- Dado una reserva Confirmada en un día posterior a hoy, cuando quien la hizo confirma la cancelación, entonces esa reserva queda Cancelada y no aparece entre las de día posterior a hoy.
- Dado una reserva Cancelada, cuando quien la hizo intenta cancelarla, entonces sigue Cancelada y ve que ya estaba cancelada.

## Fuera de alcance

- Cambiar el día, la hora o la cantidad.
- Que el local cancele una reserva.

## Supuestos

- El orden en que se muestran día, hora y cantidad no cambia el resultado de cancelar.

## Aclaraciones

- ¿Quién puede cancelar? → Solo quien hizo la reserva.
- ¿Qué pasa si ya está cancelada? → Sigue Cancelada y se ve que ya lo estaba.

## Checklist

- [x] Cada comportamiento viene de lo que el usuario dijo o de una respuesta en Aclaraciones
- [x] Cosas y Estados están escritos, aunque sea para decir que no aplican
- [x] Cada recorrido tiene empieza, hace, termina y sigue igual
- [x] Cada entonces se comprueba mirando el resultado
- [x] Cada recorrido tiene su fallo, o dice "No falla"
- [x] Fuera de alcance nombra al menos una cosa que alguien pediría
- [x] Ningún supuesto aparece como criterio
- [x] Cero marcadores `[NECESITA CLARIFICACIÓN]`
- [x] No hay nombres de framework, base de datos, API ni archivo
