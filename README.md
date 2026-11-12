# DivServices — Site officiel

Site vitrine de **DivServices** : sites web, applications de gestion et suivi technique.
Fondé par Nzouzi Exaucé Divin.

- Site en ligne : https://divservices.pages.dev
- Hébergement : Cloudflare Pages
- Code source : GitHub

## Structure

```
.
├── public/
│   └── index.html      # Le site (page unique, HTML/CSS/JS autonome)
├── wrangler.jsonc      # Configuration Cloudflare Pages
└── README.md
```

## Développement local

Ouvrir `public/index.html` dans un navigateur, ou lancer un serveur local :

```powershell
npx.cmd wrangler pages dev public
```

## Déploiement sur Cloudflare Pages

```powershell
npx.cmd wrangler login          # une seule fois
npx.cmd wrangler pages deploy public --project-name divservices
```

## Mise à jour du site

1. Modifier `public/index.html`
2. `git add . ; git commit -m "mise à jour" ; git push`
3. `npx.cmd wrangler pages deploy public --project-name divservices`

## Contact

- WhatsApp : +242 06 420 28 70
- E-mail : divservices1@gmail.com
