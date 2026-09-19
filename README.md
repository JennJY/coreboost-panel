# COREBOOST · panel de organización (Core Dumped)

Panel en vivo: https://coredumped-etsisi.github.io/2026-coreboost-panel/

Panel interno para organizar **COREBOOST**, la competición de programación de la asociación Core Dumped (ETSISI, UPM).

- Página: `index.html` (HTML estático, sin build).
- Datos en tiempo real: Firebase Realtime Database (proyecto `coreboost-e1ed5`), ruta `/coreboost`.
  - `date` — fecha del evento
  - `members/<slug>` — `{name, roles[], updatedAt}`
  - `done/<rol>_<n>` — `{by, at}` por tarea tachada
  - `budget` — `{nPart, nPodios, cont, opts{}}`
  - `notes` — notas del equipo
- Lo único local (localStorage) es "quién eres" en cada dispositivo.

Cualquiera con el enlace puede editar: es un panel de equipo, no una app pública.
