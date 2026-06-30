# 03_Map_Progression.md

# Progresión y generación del mapa

## Filosofía

Cada Run debe sentirse diferente.

Nunca debe existir un recorrido idéntico.

El jugador toma decisiones constantemente.

No existe un camino perfecto.

---

# Estructura global

Región

↓

Zona

↓

Mapa procedural

↓

Nodo

↓

Wave

↓

Recompensa

↓

Siguiente nodo

---

# Regiones

La arquitectura permitirá añadir cualquier región.

Versión inicial:

Kanto.

Cada región tiene:

Mapa propio.

Líderes.

Pokémon salvajes.

Eventos.

Tiendas.

Objetos.

Todo configurable mediante archivos JSON.

---

# Zonas

Ejemplo:

Pueblo Paleta

↓

Ruta 1

↓

Ciudad Verde

↓

Bosque Verde

↓

Ruta 2

↓

Pewter

↓

Monte Moon

↓

Ruta 4

↓

Ciudad Celeste

Cada zona constituye una pequeña Run dentro de la Run principal.

---

# Mapa procedural

Cada zona genera automáticamente:

Entre 8 y 18 nodos.

Siempre existe:

Inicio.

Final.

Al menos dos rutas distintas.

Nunca callejones sin salida.

Nunca rutas imposibles.

---

# Visibilidad

El jugador puede ver varios nodos por delante.

No puede ver el mapa completo.

Esto favorece la planificación sin eliminar la sorpresa.

---

# Tipos de nodo

Pokémon salvaje

Entrenador

Rival

Rocket

Evento

Centro Pokémon

Tienda

Tesoro

Mini Boss

Líder

Cada tipo tiene una probabilidad configurable.

---

# Waves

Las Waves representan encuentros consecutivos dentro de un mismo nodo.

Ejemplo:

Nodo Entrenador

Wave 1

Pidgeotto

↓

Wave 2

Fearow

↓

Wave 3

Raticate

↓

Recompensas

↓

Mapa

Ejemplo:

Nodo Gimnasio

Entrenador

↓

Entrenador

↓

Geodude

↓

Onix

↓

Brock

↓

Medalla

↓

Mapa

---

# Dificultad

Cada nodo aumenta ligeramente la dificultad.

Se modifica automáticamente:

Nivel.

IA.

Objetos enemigos.

Estados.

Pokémon disponibles.

Recompensas.

Todo mediante tablas de balance.

---

# Recompensas

Al finalizar un nodo el jugador elige una de varias opciones.

Ejemplo:

+ Dinero

+ Reliquia

+ Objeto

+ Poké Balls

+ Pokémon

No todas aparecen siempre.

---

# Eventos

Los eventos funcionan como pequeñas historias.

No requieren combate.

Cada evento tiene:

Texto.

Imagen.

Opciones.

Consecuencias.

Probabilidades.

Requisitos.

Todo debe definirse mediante datos.

Nunca mediante código.

---

# Fin de zona

Cada zona termina obligatoriamente con un combate importante.

Al derrotarlo:

Se obtiene la medalla.

Se desbloquea la siguiente zona.

Se guardan estadísticas.

Se genera el siguiente mapa.

---

# Escalabilidad

El sistema debe permitir añadir nuevas regiones sin modificar el motor.

Añadir Johto, Hoenn o cualquier otra región debe consistir únicamente en incorporar nuevos archivos de configuración, pools de Pokémon, eventos y mapas, reutilizando toda la lógica existente.
