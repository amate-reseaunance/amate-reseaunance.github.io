# Amate Réseaunance — site personnel de Séverine Amate

Site one-page éditorial, 100% statique (HTML/CSS/JS pur). Aucun build, aucune dépendance.

## 🚀 Hébergement gratuit — 3 options

### Option 1 — Netlify (drag & drop, le plus simple)

1. Va sur **https://app.netlify.com/drop**
2. Glisse le dossier `amatereseaunance` complet dans la zone
3. Le site est en ligne sous une URL `xxx.netlify.app` en quelques secondes
4. (Optionnel) Renomme l'URL ou branche un nom de domaine perso (`amate-reseaunance.com`) depuis le dashboard Netlify

→ **Plan gratuit suffisant** : 100 Go/mois de bande passante.

### Option 2 — Cloudflare Pages

1. Crée un compte gratuit sur **https://pages.cloudflare.com**
2. "Upload assets" → glisse le dossier
3. Tu obtiens une URL `xxx.pages.dev`

→ **Plan gratuit illimité** en bande passante.

### Option 3 — GitHub Pages

1. Crée un repo public sur GitHub (par ex. `amate-reseaunance`)
2. Push le contenu du dossier dans la branche `main`
3. Settings → Pages → Source : `main` / `/ (root)` → Save
4. URL : `https://<user>.github.io/amate-reseaunance/`

## 📁 Contenu du dossier

```
amatereseaunance/
├── index.html              ← le site
├── README.md               ← ce fichier
└── assets/
    ├── severine.jpg        ← portrait hero (à déposer)
    ├── severine-bfm.jpg    ← portrait fallback (déjà inclus, BFMTV)
    └── benoit-galy.jpg     ← portrait témoignage (à déposer)
```

Les fonts sont chargées depuis Google Fonts.

### 📸 Photos à fournir

Le site est conçu pour afficher deux portraits réels. Place les fichiers suivants dans `assets/` :

- **`severine.jpg`** — portrait carré (idéalement 800×800 px) de Séverine Amate. Recommandé : la photo iconique avec micro et fond rouge stellaire de la bannière LinkedIn — elle matche parfaitement la palette du site. À défaut, le site utilise automatiquement `severine-bfm.jpg` (déjà téléchargée depuis BFMTV).
- **`benoit-galy.jpg`** — portrait carré (idéalement 400×400 px) de Benoît Galy pour le témoignage. À défaut, le site affiche les initiales "BG" sur le gradient signature.

Format : JPG ou PNG. Le crop circulaire est géré en CSS, donc envoie un carré centré sur le visage.

## ✏️ Modifier le contenu

Tout le contenu rédactionnel se trouve dans `index.html`. Sections :

- `header.hero` — titre, slogan, CTA
- `section#manifesto` — manifeste + KPI
- `section#parcours` — timeline carrière
- `section#expertise` — 4 piliers de la méthode
- `section#case` — étude de cas Green-Acres
- `section.testimonial` — témoignage Benoît Galy
- `div.medias` — logos médias partenaires
- `section#contact` — coordonnées
- `footer` — pied de page

Pour ajouter un nouveau cas d'étude, dupliquer le bloc `section#case`. Pour modifier la palette, voir les variables CSS dans `:root` (couleurs `--coral`, `--orange`, `--fuchsia`, `--cream`, `--ink`).

## 🎨 Direction artistique

- **Typo** : Fraunces (display) + Instrument Serif (italiques) + Geist (body) + Geist Mono (méta) — toutes Google Fonts gratuites
- **Palette** : reprise du dégradé corail → orange → fuchsia de la bannière LinkedIn de Séverine
- **Slogan signature** : « Faisons parler vos datas. »

## 📱 Responsive

Optimisé desktop, tablette et mobile (testé jusqu'à 360px de large).

## ♿ Accessibilité

- Skip-to-content
- États `:focus-visible` visibles
- `prefers-reduced-motion` respecté (animations désactivées)
- Contraste AA sur tous les textes principaux
