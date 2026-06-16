# Testspecialist.nl — Website

Website voor [Testspecialist.nl](https://www.testspecialist.nl), gebouwd met [Astro](https://astro.build).

## Aan de slag

**Vereisten:** Node.js v18 of hoger

```bash
# Installeer dependencies
npm install

# Start lokale ontwikkelserver (http://localhost:4321)
npm run dev

# Bouw de productieversie
npm run build

# Bekijk de productieversie lokaal
npm run preview
```

## Projectstructuur

```
src/
├── components/
│   ├── Header.astro     # Navigatiebalk (gedeeld)
│   └── Footer.astro     # Footer (gedeeld)
├── layouts/
│   └── Layout.astro     # Hoofd-layout met <head>, header en footer
├── pages/
│   ├── index.astro      # Homepage        → /
│   ├── diensten.astro   # Diensten        → /diensten
│   ├── team.astro       # Team            → /team
│   └── contact.astro    # Contact         → /contact
└── styles/
    └── global.css       # Gedeelde stijlen en CSS-variabelen

public/
└── images/              # Afbeeldingen (logo, teamfoto's)
```

## Pagina's aanpassen

Alle pagina's staan in `src/pages/`. Elke pagina gebruikt de gedeelde `Layout.astro` en geeft een `activeNav` mee zodat het juiste menu-item actief wordt gemarkeerd.

De navigatie aanpassen doe je in `src/components/Header.astro` — één keer, geldt meteen voor alle pagina's.

## Deployen

De site kan worden gehost op [Netlify](https://netlify.com) of [Vercel](https://vercel.com), beide gratis voor statische sites.

Koppel je GitHub-repository aan Netlify of Vercel en stel de volgende build-instellingen in:

| Instelling | Waarde |
|---|---|
| Build command | `npm run build` |
| Output directory | `dist` |

Bij elke push naar de hoofdbranch wordt de site automatisch opnieuw gebouwd en gepubliceerd.
