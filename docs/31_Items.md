# Sistema de Objetos

## Filosofía

Los objetos representan decisiones tácticas durante una Run.

Nunca deben sentirse como simples consumibles.

Cada objeto debe tener un propósito claro.

Existen cuatro grandes categorías:

- Consumibles
- Equipables
- Reliquias
- Objetos clave

Cada categoría cumple una función distinta.

Nunca mezclar responsabilidades.

---

## Consumibles

Los consumibles desaparecen al utilizarlos.

Se obtienen mediante:

- Combates
- Eventos
- Tiendas
- Tesoros
- Capturas
- Misiones

---

### Curación

#### Poción

Recupera 20 PS.

#### Super Poción

Recupera 50 PS.

#### Hiper Poción

Recupera 120 PS.

#### Máxima Poción

Recupera todos los PS.

---

### Revivir

#### Revivir

Recupera el 50% de PS.

#### Revivir Máximo

Recupera el 100%.

---

### Estados

#### Antídoto

Cura Veneno.

#### Antiquemar

Cura Quemadura.

#### Antiparálisis

Cura Parálisis.

#### Despertar

Cura Sueño.

#### Antihielo

Cura Congelación.

#### Cura Total

Elimina cualquier estado.

---

## Poké Balls

Las Poké Balls son recursos muy valiosos.

Nunca deben sobrar.

Cada lanzamiento consume una unidad.

Tipos:

- Poké Ball
- Super Ball
- Ultra Ball
- Honor Ball
- Peso Ball
- Nivel Ball
- Veloz Ball
- Turno Ball
- Master Ball

Cada una modifica el cálculo de captura.

Nunca garantiza una captura salvo Master Ball.

---

## Objetos Equipables

Cada Pokémon puede equipar un único objeto.

Los objetos equipables permanecen durante toda la Run.

Ejemplos:

#### Restos

Recupera PS cada turno.

---

#### Cinta Elegida

Mayor daño.

No permite cambiar movimiento principal.

---

#### Vidasfera

Mayor ataque.

Pierde PS al atacar.

---

#### Casco Dentado

Devuelve daño.

---

#### Baya Zidra

Se consume automáticamente.

---

#### Periscopio

Mayor probabilidad crítica.

---

## Objetos Clave

No pueden venderse.

No pueden perderse.

Sirven para desbloquear contenido.

Ejemplos:

- Mapa Antiguo
- Llave Rocket
- Piedra Misteriosa
- Pase del SS Anne
- Fragmento Legendario

---

## Objetos Temporales

Solo duran una Run.

Ejemplos:

- Mapa mejorado
- Radar Pokémon
- Brújula
- Detector Shiny
- Monedero

---

## Rareza

- Común
- Poco Común
- Raro
- Épico
- Legendario
- Mítico

La rareza afecta únicamente a la frecuencia de aparición.

Nunca determina automáticamente la calidad.

---

## Tiendas

Cada tienda genera:

- Entre 4 y 8 objetos
- Entre 1 y 3 reliquias
- Entre 1 y 2 Poké Balls especiales

Nunca dos tiendas iguales.

---

## Inventario

El inventario tiene espacio limitado.

Objetivo:

Obligar al jugador a decidir.

Nunca almacenar todo.

Capacidad inicial:

20 espacios.

Puede ampliarse mediante eventos o reliquias.

---

## Uso

Los objetos pueden utilizarse:

- Durante combate
- Entre combates
- En eventos

Algunos únicamente fuera del combate.

---

## Venta

Los objetos pueden venderse.

Nunca por su valor completo.

Valor recomendado:

50%.

---

## Economía

Todo el precio de los objetos se configura mediante:

`content/balance/shop.json`

Nunca escribir precios directamente en el código.

---

## Escalabilidad

Añadir un nuevo objeto nunca debe requerir modificar el motor.

Únicamente crear un nuevo JSON con:

- ID
- Nombre
- Descripción
- Rareza
- Precio
- SVG
- Categoría
- Efectos
- Condiciones
- Animaciones

Todo debe ser interpretado automáticamente por el sistema.
