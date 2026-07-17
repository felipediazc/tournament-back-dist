# tournament-back-dist

**English** | [Español](#tournament-back-dist-español)

Distribution-only repository for **tournament-back**, the tournament management
system of the [Jhanu](https://www.jhanu.com) platform for Taekwon-Do ITF schools.
For help using the application, visit the
[support page](https://www.jhanu.com/support).

This repository contains **no source code**. It only hosts the published
application artifacts (release JARs) under
[Releases](https://github.com/felipediazc/tournament-back-dist/releases),
so the desktop launchers (`start.command` / `start.bat`) can download updates
from a public location while the application source code stays in a private
repository.

## How it works

- The private `tournament-back` repository builds the application JAR in CI.
- CI publishes each version here as a GitHub Release, attaching:
  - `tournament-back.jar`
  - `tournament-back.jar.sha256` (integrity checksum)
- The launcher checks the latest release, compares it with the locally
  installed version, and updates the JAR automatically when a newer one exists.

## Download the latest version

The latest JAR is always available at a fixed URL:

```
https://github.com/felipediazc/tournament-back-dist/releases/latest/download/tournament-back.jar
```

## Notes

- Only built artifacts live here; the source code is maintained privately.
- Released JARs are public and decompilable — they must not contain secrets.

## Support

This tool is part of the [Jhanu](https://www.jhanu.com) ecosystem. Questions,
issues or help requests: [www.jhanu.com/support](https://www.jhanu.com/support).

---

# tournament-back-dist (Español)

[English](#tournament-back-dist) | **Español**

Repositorio exclusivamente de distribución de **tournament-back**, el sistema de
gestión de torneos de la plataforma [Jhanu](https://www.jhanu.com) para escuelas
de Taekwon-Do ITF. Para ayuda con el uso de la aplicación, visita la
[página de soporte](https://www.jhanu.com/support).

Este repositorio **no contiene código fuente**. Solo aloja los artefactos
publicados de la aplicación (JARs de release) en
[Releases](https://github.com/felipediazc/tournament-back-dist/releases),
de modo que los lanzadores de escritorio (`start.command` / `start.bat`) puedan
descargar actualizaciones desde una ubicación pública mientras el código fuente
de la aplicación permanece en un repositorio privado.

## Cómo funciona

- El repositorio privado `tournament-back` construye el JAR de la aplicación en CI.
- CI publica aquí cada versión como un GitHub Release, adjuntando:
  - `tournament-back.jar`
  - `tournament-back.jar.sha256` (suma de verificación de integridad)
- El lanzador consulta el último release, lo compara con la versión instalada
  localmente y actualiza el JAR automáticamente cuando existe una más nueva.

## Descargar la última versión

El JAR más reciente está siempre disponible en una URL fija:

```
https://github.com/felipediazc/tournament-back-dist/releases/latest/download/tournament-back.jar
```

## Notas

- Aquí solo viven los artefactos compilados; el código fuente se mantiene privado.
- Los JARs publicados son públicos y descompilables — no deben contener secretos.

## Soporte

Esta herramienta es parte del ecosistema [Jhanu](https://www.jhanu.com).
Preguntas, problemas o solicitudes de ayuda:
[www.jhanu.com/support](https://www.jhanu.com/support).
