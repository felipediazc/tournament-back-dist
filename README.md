# tournament-back-dist

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
