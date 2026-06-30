# Experiencia de Combate

## Filosofía

El combate es el corazón del juego.

Debe ser el momento más divertido de toda la Run.

Cada combate debe sentirse como un combate Pokémon, no como un puzle.

El tablero es únicamente la forma en la que el entrenador da órdenes a su Pokémon.

El Pokémon es quien lucha.

No el tablero.

---

## Inicio del combate

El jugador entra en un nodo.

La cámara abandona el mapa.

Transición rápida.

El fondo cambia automáticamente según la zona.

Aparece el entrenador enemigo o el Pokémon salvaje.

Suena el grito del Pokémon.

Aparece su sprite.

Después aparece el Pokémon del jugador.

Empieza el combate.

Todo este proceso debe durar menos de tres segundos.

---

## Distribución

```text
┌────────────────────────────────────┐
        Pokémon enemigo
        Sprite animado
        Nivel
██████████████░░░░░░
        Estado
────────────────────────────────────
        TABLERO
────────────────────────────────────
        Pokémon jugador
        Sprite animado
█████████████░░░░░░
        Barra EXP
        Movimientos cargados
        Equipo
        Objetos
└────────────────────────────────────┘
```

Todo permanece siempre en la misma posición.

Nunca mover elementos durante el combate.

---

## Inicio del turno

El tablero queda desbloqueado.

El jugador puede observar.

No existe límite de tiempo.

Puede pensar.

Buscar combos.

Planificar.

---

## Movimiento

El jugador intercambia dos energías.

Si el movimiento no genera Match:

- Vuelven automáticamente.
- No consume turno.

---

## Match

Cuando existe Match:

- Las energías desaparecen.
- Se reproducen partículas.
- Se escucha el sonido correspondiente.
- Las superiores caen.
- Las inferiores se rellenan.
- Se resuelven todas las cascadas.

Solo cuando termina el tablero comienza la resolución del combate.

---

## Resolución

El motor calcula:

- Energía obtenida.
- Ataques cargados.
- Habilidades.
- Reliquias.
- Estados.
- Objetos.
- Críticos.
- STAB.
- Efectividad.

Todo ocurre automáticamente.

---

## Ataques

Cuando un movimiento está cargado:

El Pokémon realiza automáticamente su animación.

No aparece un menú preguntando.

La filosofía es mantener un ritmo alto.

Los ataques se lanzan inmediatamente.

---

## Daño

El sprite enemigo recibe un pequeño impacto.

La barra de vida disminuye suavemente.

El número aparece flotando.

Si existe crítico:

- El número vibra.

Si existe ventaja de tipo:

- Aparece el mensaje correspondiente.

Nunca detener el combate para mostrar textos largos.

---

## Estados alterados

Cuando se aplican:

- Aparece un pequeño icono.
- Una breve animación.
- El combate continúa.

No existen ventanas emergentes.

---

## Derrota del enemigo

Cuando llega a cero PS.

Pequeña animación.

El sprite desaparece.

Si existen más Pokémon:

- Aparece el siguiente.

Si no:

- Victoria.

---

## Captura

Si el enemigo puede capturarse.

Aparece el botón Poké Ball.

El combate continúa.

El jugador decide.

Nunca detener automáticamente el combate.

---

## Victoria

Experiencia.

Subidas de nivel.

Objetos.

Capturas.

Recompensas.

Todo aparece en una única secuencia fluida.

No mostrar cinco pantallas distintas.

---

## Derrota

La música cambia.

Animación.

Resumen.

Fin de la Run.

Nunca castigar al jugador con animaciones largas.

---

## Duración

- Combate salvaje: 30 a 60 segundos.
- Entrenador: 1 a 3 minutos.
- Líder: 4 a 8 minutos.
- Liga: hasta 12 minutos.

---

## Sensación

El jugador debe pensar constantemente.

Debe sentir que todas las derrotas son culpa de sus decisiones.

Nunca del azar.

Cada victoria debe sentirse merecida.

Cada derrota debe enseñar algo.
