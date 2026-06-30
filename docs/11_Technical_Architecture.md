# Arquitectura

## Filosofía

Todo el código debe ser escalable.

No existe código temporal.

No existen hacks.

Todo preparado para años de desarrollo.

---

# Stack

Next.js

TypeScript

Tailwind

Node

Neon PostgreSQL

Drizzle ORM

Zustand

PWA

---

# Arquitectura

/app

/components

/features

/game

/server

/db

/content

/hooks

/lib

/styles

/public

---

# Game Engine

Toda la lógica vive aquí.

No depende de React.

No depende del DOM.

Debe poder ejecutarse mediante tests.

---

# UI

La UI únicamente representa estados.

Nunca calcula daño.

Nunca decide resultados.

---

# Estado

Zustand.

Separado por módulos.

Run.

Combate.

Jugador.

Mapa.

Configuración.

---

# Base de datos

Neon PostgreSQL.

Toda la información importante se guarda aquí.

Usuarios.

Runs.

Historial.

Logros.

Premium.

---

# Backend

Todas las recompensas importantes se validan.

Nunca confiar en el cliente.

---

# Login

Tabla users.

Password hash.

JWT.

Cookies HttpOnly.

Rate Limit.

---

# PWA

Offline.

Instalable.

Cache.

Service Worker.

Actualización automática.

---

# Código

TypeScript estricto.

ESLint.

Prettier.

No archivos enormes.

No componentes gigantes.

No duplicación.

---

# Tests

El Game Engine debe ser testeable.

Las reglas del combate deben tener tests unitarios.

---

# Rendimiento

Objetivo.

60 FPS.

Carga menor de 2 segundos.

Sprites cacheados.

Renderizado mínimo.
