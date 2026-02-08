# AtlasHub Wiki Técnica  
Edición Open Source (Lite)

---

## Índice

- [Visión general](#visión-general)
- [Arquitectura del sistema](#arquitectura-del-sistema)
- [Flujo de ejecución](#flujo-de-ejecución)
- [Core](#core)
- [Sistema de comandos](#sistema-de-comandos)
- [Economía](#economía)
- [Juegos](#juegos)
- [Persistencia de datos](#persistencia-de-datos)
- [Panel Web](#panel-web)
- [Configuración](#configuración)
- [Seguridad y límites](#seguridad-y-límites)
- [Diferencias Lite vs Full](#diferencias-lite-vs-full)
- [Convenciones del proyecto](#convenciones-del-proyecto)
- [Contribuciones](#contribuciones)
- [Licencias](#licencias)

---

## Visión general

AtlasHub es un bot avanzado para WhatsApp desarrollado en Node.js utilizando la
librería `whatsapp-web.js`.

Esta Wiki documenta **exclusivamente** la edición **Open Source (Lite)** del
proyecto. La versión Lite está pensada para ser pública, educativa y
autohospedable.

No incluye funciones comerciales, premium ni privadas.

---

## Arquitectura del sistema

AtlasHub utiliza una arquitectura modular y desacoplada.

Componentes principales:

- `index.js`  
  Punto de entrada del bot.

- `core/`  
  Lógica central reutilizable.

- `commands/`  
  Implementación de comandos.

- `panel/`  
  Panel web local.

- `data/`  
  Persistencia de datos en JSON.

Cada capa tiene responsabilidades bien definidas.

---

## Flujo de ejecución

1. Se inicia el cliente de WhatsApp desde `index.js`.
2. Se cargan configuraciones y variables de entorno.
3. Se inicializa el core.
4. Se cargan los comandos.
5. Se inicia el panel web (si está habilitado).
6. El bot queda en estado de escucha.

Cuando llega un mensaje:

- Se valida el prefijo.
- Se identifica el comando.
- Se ejecuta la lógica correspondiente.

---

## Core

El core contiene la lógica central del sistema.

Archivos principales:

- `economy.js`  
  Manejo de balance, daily, work y perfil.

- `games.js`  
  Lógica base compartida por los juegos.

- `database.js`  
  Persistencia local en JSON.

- `commands.js`  
  Loader y gestor de comandos.

- `utils.js`  
  Funciones auxiliares comunes.

El core **no** define comandos directamente.

---

## Sistema de comandos

Cada comando es un módulo independiente.

Estructura típica de un comando:

- Nombre
- Categoría
- Descripción
- Función `execute()`

Los comandos no acceden directamente a los datos, utilizan funciones del core.

Esto permite:

- Escalabilidad
- Mantenimiento sencillo
- Código limpio

---

## Economía

La edición Lite incluye un sistema económico básico.

Funciones:

- Balance
- Daily
- Work
- Perfil de usuario

Datos almacenados por usuario:

- Balance
- Nivel
- Experiencia
- Timestamps

Existen límites internos para evitar abuso.

---

## Juegos

La edición Lite incluye juegos de azar básicos.

Lista de juegos:

- Coinflip
- Dice
- Roulette
- Higher / Lower
- Slots
- Blackjack
- Lottery

Todos los juegos:

- Usan la economía base
- No incluyen apuestas avanzadas
- No utilizan sistemas premium

---

## Persistencia de datos

AtlasHub Lite utiliza almacenamiento local mediante archivos JSON.

Características:

- Simple
- Portátil
- Sin dependencias externas

Limitaciones:

- No recomendado para grandes volúmenes
- No concurrente

---

## Panel Web

El panel web es local y opcional.

Funciones:

- Estado del bot
- Estadísticas básicas
- Ranking general

Puerto por defecto:

- `3000`

---

## Configuración

La configuración se realiza mediante el archivo `.env`.

Variables principales:

- `BOT_NAME`
- `BOT_VERSION`
- `BOT_PREFIX`
- `OWNER_ID`
- `PORT`

No se requiere configuración externa adicional.

---

## Seguridad y límites

La edición Lite:

- No maneja pagos
- No guarda información sensible
- No expone endpoints públicos

La seguridad del entorno depende del host.

---

## Diferencias Lite vs Full

### Lite

- Open Source
- Funciones básicas
- Sin monetización

### Full

- Privada
- Premium
- Comercio
- Tokens
- Multi-bot
- Panel avanzado

La versión Full **no se documenta** en esta Wiki.

---

## Convenciones del proyecto

- Arquitectura modular
- Un comando por archivo
- Core desacoplado
- Persistencia centralizada
- Prefijo configurable

---

## Contribuciones

Las contribuciones se realizan mediante Pull Requests.

Requisitos:

- Respetar la arquitectura
- No agregar funciones exclusivas de la versión Full
- Mantener el estilo del proyecto

---

## Licencias

AtlasHub se distribuye bajo licencia dual:

- MIT
- GPL-3.0

Todo código contribuido se publica bajo ambas licencias.
