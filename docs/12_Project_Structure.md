# Estructura del proyecto

## Filosofía

El proyecto debe poder mantenerse durante años.

Cualquier desarrollador debe localizar un archivo en menos de un minuto.

Nunca organizar por tipo de archivo.

Siempre organizar por Feature.

---

# Estructura

/app

    /(public)
        page.tsx
        login
        register

    /(game)
        home
        map
        battle
        shop
        profile
        settings

/components

    ui/
    shared/
    layout/
    animations/
    svg/

/features/

    auth/

    battle/

    map/

    pokemon/

    inventory/

    shop/

    rewards/

    relics/

    events/

    gyms/

    enemies/

    save/

    settings/

/game/

    engine/

    battle/

    match3/

    ai/

    map/

    rng/

    balance/

/server/

    auth/

    api/

    websocket/

/db/

    schema/

    migrations/

/content/

    regions/

    pokemon/

    trainers/

    events/

    items/

    relics/

    gyms/

    balance/

/public/

assets/

sprites/

svg/

music/

sounds/

---

# Reglas

Nunca importar directamente entre Features.

Siempre utilizar servicios.

Nunca acceder a la base de datos desde React.

Nunca mezclar lógica con UI.

Nunca guardar números mágicos.

Todo configurable.
