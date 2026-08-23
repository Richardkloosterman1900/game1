# game1

Een verzameling browserspellen, gemaakt voor Milan. Alles draait lokaal: het zijn
losse HTML-bestanden zonder server, zonder installatie en zonder bibliotheken van
buitenaf. Dubbelklik een bestand en het speelt.

## Beginnen

Open **`speelplein.html`**. Dat is de hub waar alles samenkomt.

## De bestanden

| Bestand | Wat het is |
| --- | --- |
| `speelplein.html` | Het spelplatform: 21 spellen, elk met 10 levels, plus profiel, avatar, munten, winkel en badges |
| `spookgangen.html` | First-person 3D-spel: verjaag met een zaklamp de wezens uit een donkere school |
| `neondash.html` | 3D-platformspel in Geometry Dash-stijl: de kubus rent, jij springt op de maat |
| `griezelballonnen.html` | Eerdere versie van Spookgangen, met ballonnen in plaats van wezens |

## Speelplein

**Het platform** — eigen avatar (kleuren en naam), XP en levels, munten, badges,
en per spel je record en verdiende sterren. Alles wordt in `localStorage` op de
eigen computer bewaard.

**De spellen** — Blokstapel, Slang, Reactie-rush, Doolhof, Muntenregen, Geheugen,
Steenslag, Fladderaar, Kleurcode, Ruimtewacht, Rekenraket, Hindernisbaan,
Torenklim, Blokfabriek, Schuilplaats, Rampeiland, Dierenopvang, Kluiskraker,
Honderd deuren, Sprintbaan en Duwarena.

**Levels** — elk spel heeft er tien. Haal het doel om het volgende te openen; ga
ver over het doel heen voor twee of drie sterren.

**De winkel** — met je munten koop je hulpmiddelen die je per potje inzet: een
schild dat één fatale fout opvangt, extra tijd, een vertrager, dubbele punten,
een magneet en een wegwijzer.

## Onder de motorkap

De 3D-spellen gebruiken geen 3D-bibliotheek. `spookgangen.html` heeft een eigen
raycasting-engine met procedureel gebakken texturen, zaklampverlichting en een
renderresolutie die zich aan de snelheid van de computer aanpast.
`neondash.html` heeft een eigen polygonenrenderer met perspectiefprojectie en
dieptesortering. Al het geluid wordt live met de Web Audio API gemaakt.
