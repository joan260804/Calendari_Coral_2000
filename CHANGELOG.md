# Calendari activitats Coral 2000 · Registre de versions

Es fa servir el sistema **MAJOR.MINOR.PATCH** (per exemple, `1.0.0`):

| Número | Quan es puja | Exemple |
|---|---|---|
| **MAJOR** (1.0.0 → 2.0.0) | Canvis grans o que obliguen a fer les coses d'una altra manera | Nou sistema d'accés, canvi total de disseny |
| **MINOR** (0.1.0 → 0.2.0) | Funcionalitat nova que no trenca res | Un camp nou als events, un nou tipus d'avís |
| **PATCH** (0.1.0 → 0.1.1) | Correccions i retocs petits | Errors, textos, mides, colors |

Mentre el MAJOR sigui `0`, l'aplicació és en fase de prova pilot. Quan s'aprovi per a tothom, es passa a `1.0.0`.

## Com publicar una versió nova
1. A `index.html`, canvia **només** la línia `const APP_SEMVER = '0.1.0';` pel número nou.
2. Afegeix una entrada a aquest fitxer (a dalt de tot).
3. Puja `index.html` (i aquest fitxer) a GitHub: *Add file → Upload files → Commit changes*.
4. Les aplicacions instal·lades es comproven soles en obrir-se i s'actualitzen si hi ha una versió més alta.

> No toquis la línia `const APP_VERSION = 43;`: és un residu perquè les còpies antigues (numerades amb enters) s'actualitzin una sola vegada.

---

## 0.1.0 · Versió pilot inicial
Primera versió presentada als editors i als usuaris.

**Accés i permisos**
- Entrada amb el número de telèfon; rols de lectura i d'editor.
- Els editors entren a més amb contrasenya (amb icona d'ull) i poden restablir-la per correu.

**Calendari**
- Vista mensual amb lletra gran: dies amb activitat en verd, festius en vermell i avui en blau.
- Festius oficials de Catalunya i festes locals de Terrassa (2026 i 2027; Terrassa 2027 pendent).
- Selector de mes i any; títol centrat en dues línies.

**Activitats (només editors)**
- Crear, editar i esborrar activitats amb títol, comentari (128 car.), ubicació de Google Maps, dates i hores.
- Repeticions estil Google Calendar (dia, setmana, mes, any); s'ometen els dies festius.
- Esborrar amb motiu (128 car.) i opcions «només aquest / aquest i els següents / tots».

**Avisos**
- En crear o cancel·lar una activitat es pot enviar un missatge preparat al grup de WhatsApp.

**Instal·lació**
- Icona a la pantalla d'inici (Android i iPhone), vista prèvia en compartir l'enllaç i actualització automàtica.
