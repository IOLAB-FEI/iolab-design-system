# IoLab Design System

Statický design system + logo set pre [iolab.sk](https://iolab.sk).

## Obsah

- **`design-system.html`** — kompletný design system: farebné tokeny, surface tiers, typografia, komponenty (tlačidlá, inputy, chips, karty, alerty), demo appka, sťahovateľný Vuetify 3 config.
- **`logo.html`** — logo set s 6 variantami (Base, Full, Horizontálny, Tričko 1/2 riadky, Favicon), 4 farebnými podkladmi, exportom do SVG (jednotlivo aj batch) a PNG v rôznych veľkostiach (512–6000 px).
- **`index.html`** — landing page s odkazmi na obe stránky.

Oba dokumenty sú **plne self-contained** — jediná externá závislosť je Google Fonts CDN (DM Sans + DM Mono). Žiadny build step, žiadne npm, žiadne frameworky. Stačí otvoriť v prehliadači alebo nahrať na webserver.

## Live verzia

Po zapnutí GitHub Pages bude dostupné na:

```
https://jakubmatisak.github.io/iolab-design-system/
```

Settings → Pages → Source: `Deploy from a branch` → `main` / `root`.

## Lokálny vývoj

```bash
git clone https://github.com/jakubmatisak/iolab-design-system.git
cd iolab-design-system
python3 -m http.server 8000
# otvor http://localhost:8000
```

## Vuetify 3 integrácia

V design systeme nájdeš tlačidlo **„Stiahnuť config"** ktoré ti stiahne `vuetify.js` súbor — paste ho do `plugins/vuetify.js` v tvojej Vue/Nuxt appke a máš kompletné Material 3 theming s IoLab farbami (navy primary, cyan tertiary), light + dark theme, defaults pre VBtn, VCard, VTextField, VChip, atď.

## Farebné role

| Token | Light | Dark |
|---|---|---|
| `primary` | `#1e2a4a` navy | `#fefefe` |
| `secondary` | `#475569` slate | `#dae2fd` |
| `tertiary` | `#86dad3` cyan | `#8fe3dc` |
| `error` | `#ba1a1a` | `#ffb4ab` |
| `warning` | `#a05f0c` | `#ffc88c` |
| `info` | `#3b6bd0` | `#b0c6ff` |
| `success` | `#3fa888` | `#82d4b7` |

## Logo varianty

- **A · Base** — len ikona (io · LAB stack)
- **B · Full** — ikona + text "IoLab" + tagline
- **C · Horizontálny** — ikona vedľa textu
- **D₁ · Tričko 1 riadok** — pre printovanie, kompaktné
- **D₂ · Tričko 2 riadky** — s rozvinutým taglinom
- **Favicon** — štvorcový crop

Všetky varianty exportovateľné v 4 farebných variantoch (cream, white, ink dark, cyan).

## License

© IoLab. Logo a brand assets sú vyhradené pre IoLab. Kód komponentov je voľne použiteľný pre vlastné projekty.
