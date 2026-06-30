# Gameplay

### Objetivo del jugador

Cada partida (Run) representa una aventura completa por una versión condensada de Kanto.

El jugador comienza sin progreso dentro de la Run y debe construir un equipo capaz de derrotar a todos los Líderes de Gimnasio hasta llegar a la Liga Pokémon.

Al perder todos sus Pokémon la Run termina.

No existe guardado manual.

La Run se guarda automáticamente después de cada acción importante.

### Estructura general de una Run

```text
Inicio
↓
Elegir Pokémon inicial
↓
Mapa de Kanto
↓
Elegir siguiente nodo
↓
Resolver evento del nodo
↓
Obtener recompensa
↓
Volver al mapa
↓
Repetir
↓
Líder de Gimnasio
↓
Siguiente zona
↓
...
↓
Liga Pokémon
↓
Victoria
```

### Regiones

El juego se divide en regiones.

La primera versión únicamente contiene Kanto.

Cada región está formada por varias zonas.

Ejemplo:

- Pueblo Paleta
- Ruta 1
- Ciudad Verde
- Bosque Verde
- Ruta 2
- Pewter
- Monte Moon
- Ruta 4
- Ciudad Celeste
- ...

Cada zona termina con un combate importante.

### Estructura de una zona

Cada zona está formada por un pequeño mapa procedural.

Duración estimada: 5 a 12 minutos.

El jugador debe recorrer varios nodos antes de llegar al combate final.

Ejemplo:

```text
Inicio
↓
Pokémon Salvaje
↓
Entrenador
↓
Evento
↓
Centro Pokémon
↓
Pokémon Salvaje
↓
Tienda
↓
Líder
```

Cada Run modifica este recorrido.

### Mapa

El mapa ocupa prácticamente toda la pantalla.

Cada nodo está conectado mediante líneas.

El jugador únicamente puede avanzar.

Nunca retroceder.

Siempre existen entre dos y tres caminos posibles.

El jugador puede ver varios nodos por delante para planificar su ruta.

### Tipos de nodo

#### Combate Salvaje

El combate más común.

Sirve para ganar experiencia, conseguir dinero, capturar Pokémon y encontrar objetos.

Duración: 30 a 90 segundos.

#### Entrenador

Mayor dificultad.

Equipos de entre 2 y 6 Pokémon.

Mayor recompensa.

Mayor experiencia.

#### Rival

Combates especiales.

El rival aparece varias veces durante la Run.

Su equipo evoluciona igual que el jugador.

Puede sorprender con estrategias diferentes.

#### Team Rocket

Nodo especial.

Cada combate incluye una regla adicional.

Ejemplos:

- El tablero tiene bloques.
- El jugador empieza envenenado.
- Las fichas oscuras aparecen con mayor frecuencia.
- Cada tres turnos aparece una bomba.

Cada combate Rocket puede sentirse diferente.

#### Centro Pokémon

Recupera completamente:

- PS
- Estados alterados
- PP si existen

No ofrece recompensa económica.

#### Tienda

Permite gastar monedas.

Comprar:

- Poké Balls
- Pociones
- Revivir
- Bayas
- Objetos permanentes
- Reliquias

No todas las tiendas ofrecen el mismo catálogo.

#### Evento

No existe combate.

Se presenta una situación.

El jugador debe decidir.

Ejemplo:

```text
Encuentras una mochila abandonada.

Abrirla.
Ignorarla.
Robarla.
```

Cada decisión tiene consecuencias buenas, malas o impredecibles.

#### Tesoro

Entrega recompensas gratuitas.

Puede contener:

- Objetos
- Dinero
- Poké Balls
- Reliquias
- Pokémon raro

#### Gimnasio

Último nodo de la zona.

Es obligatorio.

Siempre termina la zona.

No existe otro camino.

### Recompensas

Después de cada combate el jugador recibe una combinación de:

- Experiencia
- Dinero
- Objetos
- Poké Balls
- Nuevos Pokémon
- Reliquias
- Mejoras permanentes para la Run

Nunca dos recompensas idénticas.

### Captura de Pokémon

Los Pokémon salvajes pueden capturarse.

No todos.

Cada especie tiene una probabilidad.

El jugador necesita Poké Balls.

La captura únicamente puede intentarse cuando el rival tenga poca vida.

Al capturarlo:

- Se añade al equipo.
- O se envía a la reserva.

Nunca desaparece el combate automáticamente.

### Equipo

Máximo: 6 Pokémon.

Durante el combate únicamente participa uno.

Entre combates el jugador puede reorganizar el equipo.

Cambiar posiciones.

Curar.

Equipar objetos.

### Evoluciones

Los Pokémon evolucionan automáticamente al alcanzar el nivel correspondiente.

No se cancela la evolución.

Las evoluciones por piedra requieren disponer del objeto.

Las evoluciones especiales podrán implementarse más adelante.

### Fin de la Run

La Run termina cuando todos los Pokémon son derrotados o se derrota a la Liga Pokémon.

Al finalizar aparece un resumen completo:

- Tiempo
- Pokémon utilizados
- Combates
- Capturas
- Dinero ganado
- Daño realizado
- Objetos usados
- Nodos recorridos
- Shinies encontrados
- Récords
- Experiencia de cuenta
- Logros obtenidos

Después el jugador vuelve al menú principal.
