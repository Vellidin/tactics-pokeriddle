# Arquitectura de contenido

## Filosofía

Todo el contenido del juego debe ser configurable.

Nunca modificar código para añadir contenido.

El motor debe leer archivos de configuración.

---

## Estructura

```text
/content
├── regions/
├── pokemon/
├── moves/
├── items/
├── events/
├── gyms/
├── shops/
├── weather/
├── terrain/
├── enemyTeams/
├── relics/
├── balance/
└── locales/
```

---

## Regiones

Cada región posee un archivo.

Ejemplo:

- `kanto.json`
- `johto.json`
- `hoenn.json`

Cada uno define:

- Orden.
- Zonas.
- Pokémon.
- Eventos.
- Objetos.
- Líderes.
- Pools.

---

## Zonas

Cada zona define:

- Nombre.
- Nivel mínimo.
- Nivel máximo.
- Pokémon salvajes.
- Entrenadores.
- Clima.
- Terrenos.
- Música.
- Imagen de fondo.
- Tipos de nodo.

---

## Pokémon

Cada especie tiene un archivo.

Incluye:

- ID PokeAPI.
- Tipos.
- Estadísticas.
- Habilidades.
- Movimientos.
- Evoluciones.
- Sprites.
- Animaciones.
- Rareza.

---

## Equipos enemigos

Cada entrenador posee:

- Nombre.
- Avatar.
- Equipo.
- Objetos.
- IA.
- Frases.
- Recompensas.

No existen equipos hardcodeados.

---

## Eventos

Cada evento es independiente.

Ejemplo:

- id
- titulo
- texto
- imagen
- condiciones
- opciones
- probabilidades
- resultado
- recompensas

Todo configurable.

---

## Objetos

Cada objeto define:

- Nombre.
- Descripción.
- Rareza.
- Precio.
- Icono SVG.
- Uso.
- Duración.
- Efectos.

No existe lógica específica dentro del objeto.

Todo utiliza un sistema de efectos.

---

## Reliquias

Las reliquias modifican la Run.

Ejemplos:

- +10% experiencia.
- Las capturas son más fáciles.
- Empiezas con una Poción.
- Las energías Planta generan un punto extra.

Todas deben implementarse mediante modificadores.

---

## Balance

Todo el balance vive en archivos separados.

- `exp.json`
- `damage.json`
- `economy.json`
- `shops.json`
- `enemyScaling.json`
- `capture.json`

Nunca utilizar números escritos directamente en el código.

---

## Temporadas

El juego debe soportar temporadas.

Cada temporada puede añadir:

- Eventos.
- Objetos.
- Skins.
- Recompensas.
- Fondos.
- Música.

Sin modificar el motor.

---

## Eventos especiales

Halloween.

Navidad.

Aniversario.

Verano.

Todos utilizan el mismo sistema.

Simplemente activando contenido.

---

## Localización

Todo el texto debe utilizar i18n.

Nunca escribir texto directamente en componentes.

Idiomas iniciales:

- Español.
- Inglés.
- Francés.
- Italiano.
- Portugués.

---

## Recursos

Toda la información Pokémon proviene de:

- PokeAPI
- PokeAPI Resources

Nunca almacenar sprites duplicados.

Siempre cachear.

Siempre utilizar recursos oficiales cuando existan.

---

## Escalabilidad

Añadir una nueva región debe consistir únicamente en:

- Crear un archivo de región.
- Añadir Pokémon.
- Añadir entrenadores.
- Añadir eventos.
- Añadir líderes.

El motor no debe modificarse.

Ese es el objetivo principal de la arquitectura.
