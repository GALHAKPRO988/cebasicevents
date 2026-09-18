# CONDITIONAL EVENTS BASIC EVENTS (TEMPLATES)

**DISCLAIMER: Esto fue creado por la comunidad, no es oficial. Recuerda siempre usar la wiki cuando hagas tus propios eventos. Nosotros no damos soporte del plugin. Estos son eventos MUY MUY básicos que solo son recomendables como templates para aquellos que acaban de empezar a usar el plugin.**

Colección de templates listos para usar con el plugin **ConditionalEvents** (by ajneb97) para servidores Spigot/Paper.

Cada archivo `.yml` define uno o más eventos que puedes copiar dentro del bloque de eventos de tu `config.yml` del plugin, o cargarlos como referencia y adaptarlos a tu servidor.

📖 Documentación oficial del plugin: https://ajneb97.gitbook.io/conditionalevents
🔌 Página del plugin: https://www.spigotmc.org/resources/82271/

## Requisitos

- Spigot o Paper (no Craftbukkit).
- [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) — recomendado, necesario para variables como `%worldguard_region_name%` o `%target:vault_rank%`.
- Vault + un plugin de economía (EssentialsX, etc.) si usas los eventos de `economia/` (usan `eco give` por consola).
- WorldGuard si usas `moderacion/patrulla_zona_prohibida.yml`.

## Estructura del repositorio

| Carpeta | Contenido |
|---|---|
| `boxpvp/` | `cobweb_temporal.yml` — al colocar una tela de araña, se borra sola tras unos segundos. |
| `player/` | `night_vision_mundo.yml` — visión nocturna constante en un mundo concreto. |
| `moderacion/` | Bloqueo de comandos peligrosos, protección de bloques en spawn, patrulla de zona prohibida. |
| `economia/` | Comandos secretos que dan diamantes o dinero, recompensa por kill según rango, logro por minar. |
| `bloques/` | Botón que da dinero al pulsarlo, sin daño por caída en spawn. |
| `diversion/` | Fuegos artificiales aleatorios por comando, mensaje de bienvenida. |

## Cómo usar un template

1. Abre el archivo `.yml` que te interese.
2. Copia el bloque del evento (todo lo que empieza en el nombre del evento, ej. `cobweb_temporal:`) dentro de la sección de eventos de tu `config.yml` de ConditionalEvents.
3. Ajusta los valores de ejemplo (nombres de mundo, coordenadas, cantidades, nombres de comando) a los de tu servidor.
4. Recarga el plugin (`/ce reload` o el comando equivalente) o reinicia el servidor.

## Notas

- Todos los nombres de mundo (`spawn`, `minas`, `lobby`, `zona_prohibida`) son de ejemplo: cámbialos por los tuyos.
- `ignore_with_permission` permite que el staff con ese permiso salte la restricción del evento.
- Puedes apilar varias acciones dentro de `default:` para dar más de una recompensa o efecto a la vez.
- Antes de subir un evento nuevo a este repo, verifica su sintaxis contra la documentación oficial enlazada arriba.

## Contribuir

Pull requests bienvenidas: añade tu archivo `.yml` en la carpeta que corresponda (o crea una nueva si no encaja en ninguna) y describe brevemente qué hace en un comentario al inicio del archivo.
