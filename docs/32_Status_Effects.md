# Sistema de Estados Alterados

## Filosofía

Los estados alterados no son únicamente penalizaciones.

Cambian la forma de jugar.

Cada estado debe obligar al jugador a adaptar su estrategia.

Todos los estados utilizan un sistema común basado en modificadores.

Nunca crear lógica específica para cada estado.

Todo debe definirse mediante datos.

---

## Estructura

Cada estado define:

- ID
- Nombre
- Descripción
- Icono SVG
- Color
- Duración
- Acumulable
- Animación
- Sonido
- Prioridad
- Efectos
- Condiciones
- Contramedidas

---

## Veneno

Daño al finalizar cada turno.

Puede acumularse dependiendo del origen.

Color principal:

Morado.

---

## Quemadura

Reduce el ataque físico.

Produce daño residual.

Color:

Rojo.

---

## Parálisis

Puede impedir actuar.

Reduce la velocidad.

Produce pequeñas descargas visuales.

---

## Sueño

Impide actuar.

Puede despertarse automáticamente.

Algunos ataques pueden despertarlo.

---

## Congelación

Impide actuar.

Puede romperse con ataques de fuego.

---

## Confusión

Existe una probabilidad de golpearse a sí mismo.

No impide actuar siempre.

---

## Maldición

Pierde vida constantemente.

Aumenta el daño realizado.

Ideal para Builds de riesgo.

---

## Miedo

El Pokémon no puede utilizar ataques cuyo coste supere cierta cantidad de energía.

---

## Silencio

Impide utilizar habilidades especiales.

Los ataques básicos siguen funcionando.

---

## Sangrado

Cada Match realizado produce daño adicional al propio Pokémon.

Muy peligroso.

---

## Drenado

Cada ataque cura al enemigo.

---

## Debilidad

El daño recibido aumenta.

---

## Fortaleza

El daño recibido disminuye.

---

## Escudo

Absorbe una cantidad fija de daño.

Puede acumularse.

---

## Estados Positivos

No todos los estados son negativos.

Ejemplos:

#### Inspiración

Más energía obtenida.

---

#### Concentración

Mayor probabilidad crítica.

---

#### Regeneración

Recupera PS cada turno.

---

#### Velocidad

Permite generar más energía por Match.

---

#### Protección

Reduce el siguiente ataque recibido.

---

## Climas

Los climas afectan a todo el combate.

#### Lluvia

Agua +25%.

Fuego -25%.

---

#### Sol intenso

Fuego +25%.

Agua -25%.

---

#### Tormenta arena

Daño residual.

Los Pokémon Roca son inmunes.

---

#### Granizo

Daño residual.

Los Pokémon Hielo son inmunes.

---

#### Niebla

Reduce precisión.

---

## Terrenos

#### Campo eléctrico

Las energías Eléctricas generan más energía.

---

#### Campo de hierba

Curación ligera.

---

#### Campo psíquico

Mayor generación de energía Psíquica.

---

#### Campo bruma

Reduce estados alterados.

---

## Obstáculos del tablero

Los obstáculos también pueden actuar como estados.

#### Raíz

Bloquea una casilla.

---

#### Roca

Debe destruirse.

---

#### Hielo

Necesita varios impactos.

---

#### Cadena

Impide mover una energía.

---

#### Veneno

Las energías que pasan por esa casilla quedan contaminadas.

---

#### Bomba Rocket

Explota tras varios turnos.

---

#### Cristal

Puede romperse para obtener recompensas.

---

## Interacciones

Los estados pueden combinarse.

Ejemplos:

#### Veneno + Quemadura

Mayor daño residual.

---

#### Lluvia + Eléctrico

Las energías eléctricas afectan a más casillas.

---

#### Sol + Planta

Mayor curación.

---

#### Arena + Roca

Mayor defensa.

Todo debe ser configurable mediante archivos JSON.

Nunca codificado manualmente.
