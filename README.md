# Alohins Webz

Personlig nettside for Alohins Webz — bygget med Astro 5 og Geist Variable.

🌐 **Live:** [alohins-webz.no](https://alohins-webz.no)

---

## Lokal utvikling

Krever Node.js 20+.

```bash
npm install     # installer avhengigheter (én gang)
npm run dev     # start utviklingsserver på http://localhost:4321
npm run build   # bygg for produksjon (output i dist/)
npm run preview # forhåndsvis produksjonsbygget lokalt
```

---

## Struktur

```
src/
├── styles/         # tokens.css + global.css (designsystem)
├── layouts/        # Layout.astro (HTML-skall + SEO)
├── components/     # Nav, Hero, Services, Approach, Projects,
│                     Testimonials, Compare, Pricing, Maintenance,
│                     About, Contact, Footer, Logo, Button
└── pages/
    └── index.astro # forsiden — setter sammen seksjonene
public/             # statiske ressurser (favicon, logo, prosjektbilder)
```

---

## Designsystem

Alle farger, font-størrelser, mellomrom og avrundinger er CSS-variabler i `src/styles/tokens.css`. Endre én verdi der, og hele nettsiden følger med.

**Hovedpalett:**
- Bakgrunn: `#FAF7F2` (varm krem)
- Tekst: `#1A1A1A` (nesten svart)
- Aksent: `#C75B3C` (terrakotta)

**Skrift:** Geist Variable (én skrift, alle vekter)

---

## Deployment

Automatisk via GitHub → Hostinger (Cloud Startup).
Push til `main`-branchen utløser ny build på serveren.

Build command: `npm run build`
Output directory: `dist`
