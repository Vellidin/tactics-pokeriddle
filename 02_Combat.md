# Sistema de Combate

## Objetivo

El combate debe transmitir la sensación de un combate Pokémon tradicional, pero sustituyendo la selección de movimientos por un tablero Match-3.

El jugador debe sentir que controla el combate constantemente.

Nunca debe existir un turno en el que simplemente observe sin interactuar durante demasiado tiempo.

La duración ideal de un turno completo (jugador + enemigo) es de entre 3 y 8 segundos.

---

## Presentación

El combate ocupa toda la pantalla.

```text
┌─────────────────────────────────────────────┐

            Pokémon enemigo

          Sprite animado

       Lv.18

████████████████████░░░

PS 134 / 180

Estado: Quemado

─────────────────────────────────────────────

           TABLERO MATCH-3

─────────────────────────────────────────────

            Tu Pokémon

          Sprite animado

       Lv.19

███████████████░░░░░░

PS 102 / 145

EXP ████████░░░░░░

Equipo (6)

Objetos

Huir (si está permitido)

└─────────────────────────────────────────────┘
```

---

## Flujo del combate

```text
Inicio
↓
Animación de entrada
↓
Presentación de entrenadores (si existe)
↓
Aparece el tablero
↓
Turno del jugador
↓
Resolución de combos
↓
Aplicación de daño
↓
Estados alterados
↓
Turno enemigo
↓
Aplicación del movimiento enemigo
↓
Nuevo turno
```

---

## Turno del jugador

El jugador únicamente puede realizar un movimiento.

Al intercambiar dos fichas se bloquea el tablero.

Se resuelven automáticamente:

- Match principal
- Combos
- Cascadas
- Habilidades
- Estados

Solo cuando todo termina el enemigo actúa.

---

## Tipos de ficha

Cada ficha representa un tipo Pokémon.

- Planta
- Fuego
- Agua
- Eléctrico
- Roca
- Tierra
- Hielo
- Psíquico
- Lucha
- Volador
- Fantasma
- Dragón
- Siniestro
- Acero
- Hada
- Veneno
- Bicho
- Normal

Las fichas utilizan iconografía SVG.

Nunca texto.

Nunca emojis.

---

## Daño

El daño depende de:

- Longitud del Match.
- Tipo de ficha.
- Ataque del Pokémon.
- Defensa rival.
- STAB.
- Efectividad.
- Críticos.
- Objetos.
- Estados.
- Nivel.

Nunca existe un daño fijo.

Todo debe calcularse mediante fórmulas configurables.

---

## Combos

Un Match puede provocar:

- Caída de fichas.
- Nuevos Match.
- Cadena.

Cada nuevo Match aumenta un multiplicador.

Ejemplo:

```text
Combo x2
Combo x3
Combo x4
```

Cada combo incrementa ligeramente el daño.

---

## Animaciones

Al romper fichas:

- Las fichas desaparecen.
- Se reproducen partículas.
- Las superiores caen.
- Se generan nuevas.

Cuando termina el tablero:

- Se calcula el daño.
- El sprite enemigo recibe impacto.
- La barra de vida disminuye suavemente.
- Aparecen números flotantes.

Si el ataque es:

- Muy eficaz.
- Poco eficaz.
- Crítico.
- Inmune.

Debe mostrarse un indicador visual.

---

## Estados alterados

Los estados alterados permanecen durante varios turnos.

- Quemado
- Veneno
- Parálisis
- Sueño
- Congelado
- Confusión

Quemado reduce daño y causa daño residual.

Veneno causa daño al finalizar turno.

Parálisis puede impedir mover.

Sueño impide actuar varios turnos.

Congelado puede descongelarse.

Confusión puede dañarse a sí mismo.

Todos deben implementarse mediante un sistema de efectos configurable.

---

## Cambio de Pokémon

Cuando un Pokémon cae debilitado:

- Animación KO.
- El jugador selecciona el siguiente.
- La batalla continúa.

Si no quedan Pokémon:

- Fin de la Run.

---

## Victoria

- Animación.
- Experiencia.
- Dinero.
- Captura (si procede).
- Objetos.
- Recompensas.
- Regreso al mapa.

---

## Derrota

- Todos los Pokémon debilitados.
- Pantalla de derrota.
- Resumen completo.
- Fin de la Run.

---

## Objetivos de diseño

Los combates deben sentirse:

- Rápidos.
- Muy visuales.
- Tácticos.
- Fluidos.
- Satisfactorios.

Nunca lentos.

Nunca repetitivos.

Nunca depender exclusivamente de la suerte.
