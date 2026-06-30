# Match-3 Engine

## Filosofía

El tablero no representa un simple puzle.

Representa el campo de batalla donde ambos Pokémon luchan.

Cada movimiento debe sentirse importante.

Nunca debe existir un Match "porque sí".

El jugador siempre debe pensar varios movimientos por delante.

---

## Tamaño

El tablero utiliza:

- 8 columnas.
- 8 filas.
- 64 casillas.

Todas las casillas tienen el mismo tamaño.

El tablero ocupa aproximadamente el 60% de la pantalla.

---

## Energías

Las fichas pasan a llamarse Energías.

Cada energía representa un tipo Pokémon.

- Planta
- Fuego
- Agua
- Eléctrico
- Hielo
- Roca
- Tierra
- Veneno
- Fantasma
- Lucha
- Normal
- Volador
- Bicho
- Psíquico
- Dragón
- Acero
- Hada
- Siniestro

Las energías utilizan únicamente iconografía SVG.

Nunca texto.

Nunca emojis.

---

## Generación

El tablero nunca puede generarse con:

- Matches automáticos.
- Tableros imposibles.

Siempre debe existir al menos un movimiento válido.

Si no existe:

- Se mezcla automáticamente.

---

## Match

### 3 energías

Carga básica.

### 4 energías

Carga adicional.

Genera una energía especial.

### 5 energías

Gran carga.

Explosión.

Mayor daño.

---

## Cascadas

Cuando desaparecen energías:

- Las superiores caen.
- Se rellenan automáticamente.

Las nuevas pueden provocar:

- Nuevos Match.
- Combos.
- Multiplicadores.

Todo se resuelve automáticamente.

---

## Multiplicador

Cada Match consecutivo aumenta:

- Combo x2
- Combo x3
- Combo x4
- ...

El multiplicador incrementa:

- Daño.
- Carga.
- Experiencia del combate.

---

## Energías especiales

Existen energías especiales.

### Energía Bomba

Explota alrededor.

### Energía Rayo

Elimina una fila.

### Energía Columna

Elimina una columna.

### Energía Arcoíris

Cuenta como cualquier tipo.

Estas pueden aparecer mediante:

- Match de cinco.
- Habilidades.
- Objetos.
- Eventos.

---

## Obstáculos

Los obstáculos ocupan casillas.

No pueden moverse.

Ejemplos:

- Rocas.
- Lianas.
- Hielo.
- Cadenas.
- Veneno.
- Arena.
- Electricidad.

Cada obstáculo posee reglas distintas.

---

## Objetos del escenario

Algunos escenarios generan elementos propios.

### Poké Ball

Al romperla puede contener:

- Dinero.
- Objeto.
- Pokémon.
- Nada.

### Baya

Recupera vida.

### Caja Rocket

Puede explotar.

### Cristal

Otorga experiencia.

### Fósil

Entrega reliquias.

---

## Clima

Algunos combates tienen clima.

- Lluvia.
- Sol intenso.
- Tormenta arena.
- Granizo.
- Niebla.

Cada clima modifica:

- Daño.
- Energías.
- Generación.
- Estados alterados.

---

## Terreno

También pueden existir terrenos.

- Campo eléctrico.
- Campo de hierba.
- Campo psíquico.
- Campo bruma.

Funcionan durante varios turnos.

---

## Eventos del tablero

Cada combate puede tener reglas especiales.

Ejemplos:

- Cada tres turnos aparecen rocas.
- Cada dos turnos se congelan casillas.
- Las energías oscuras generan veneno.
- Las energías fuego explotan.
- Las energías agua curan.

Todo configurable.

Nunca mediante código.

---

## IA

La IA también interactúa con el tablero.

No hace trampas.

No modifica energías.

Simplemente utiliza habilidades.

Estados.

Objetos.

Cambios de Pokémon.

---

## Rendimiento

Todo el tablero debe ejecutarse a 60 FPS.

Las animaciones nunca bloquearán la entrada del jugador.

Toda la lógica será independiente del renderizado.

---

## Objetivo

El tablero debe sentirse vivo.

No como una cuadrícula.

Sino como un combate Pokémon donde el escenario también participa.
