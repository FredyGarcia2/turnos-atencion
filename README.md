# turnia. · Sistema de turnos para atención a clientes

Aplicación web para organizar la atención a clientes mediante turnos: el cliente toma su número, el asesor lo llama desde una mesa y una pantalla en la sala lo anuncia.

**Demo:** https://turnos-swart.vercel.app

## Vistas

| Vista | Ruta | Para qué sirve |
|---|---|---|
| Control de turnos | `/#panel` | Panel del asesor: fila de espera, mesas, llamar siguiente, finalizar atención y actividad reciente. |
| Pantalla de sala | `/#sala` | Pantalla pública con el turno llamado, el estado de las mesas y anuncio por voz. |
| Kiosko | `/#kiosko` | El cliente elige el servicio y recibe su turno con posición y tiempo estimado. |

## Características

- Cuatro servicios (A, B, C, D) con numeración propia, por ejemplo `A029`.
- Cuatro mesas de atención que llaman al siguiente turno en orden.
- Anuncio por voz en la pantalla de sala.
- Diseño responsive: menú lateral en escritorio y barra inferior en celular.
- Modo claro y oscuro automático.
- Sin dependencias: un solo archivo HTML con CSS y JavaScript.

## Tecnologías

HTML, CSS y JavaScript puro. Los datos se guardan en el navegador (`localStorage`) y se sincronizan entre pestañas del mismo equipo. Desplegado en Vercel.

## Uso local

Abre `index.html` en el navegador. No requiere instalación.

## Despliegue

Cada `git push` a la rama `main` se publica automáticamente en Vercel.
