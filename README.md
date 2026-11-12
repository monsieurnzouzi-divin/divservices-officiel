# DivServices — Site officiel

Site vitrine de **DivServices** : sites web, applications de gestion et suivi technique.
Fondé par Nzouzi Exaucé Divin.

- Site en ligne : https://divservices.pages.dev
- Hébergement : Cloudflare Pages
- Code source : https://github.com/monsieurnzouzi-divin/divservices-officiel

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

## Déploiement

Le projet Cloudflare Pages **`divservices`** est connecté au dépôt GitHub.
Chaque `git push` sur la branche `main` déclenche automatiquement un build et
une mise en ligne (aucune commande de déploiement à lancer).

| Réglage Cloudflare Pages | Valeur |
|---|---|
| Dépôt | `monsieurnzouzi-divin/divservices-officiel` |
| Branche de production | `main` |
| Commande de build | *(vide)* |
| Dossier de sortie | `public` |
| Dossier racine | *(vide)* |

## Mise à jour du site

1. Modifier `public/index.html`
2. `git add . ; git commit -m "mise à jour" ; git push`
3. Attendre ~1 minute : le site est à jour sur https://divservices.pages.dev

### Déploiement manuel (secours)

Si besoin de publier sans passer par Git :

```powershell
npx.cmd wrangler pages deploy public --project-name divservices
```

> ⚠️ Ne pas utiliser cette commande en usage courant : elle crée un déploiement
> hors Git, qui sera écrasé au prochain `git push`.

## Projets Cloudflare liés

| Projet | Rôle |
|---|---|
| `divservices` | Site officiel (ce dépôt) |
| `divservices-school` | Application de gestion d'école — dépôt séparé, indépendant |

## Contact

- WhatsApp : +242 06 420 28 70
- E-mail : divservices1@gmail.com
