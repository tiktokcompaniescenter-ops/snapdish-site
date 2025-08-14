# Déployer le site SnapDish

Ce dossier contient une **vitrine prête à publier** :
- `index.html`
- `assets/snapdish-logo-base.png` (logo de remplacement, à remplacer par votre logo final)

## Option A — Netlify (recommandé : très simple + formulaires natifs)

1. Créez un compte sur https://app.netlify.com/
2. Glissez-déposez le dossier **/site** dans *Sites* → *Add new site* → *Deploy manually*
3. Le formulaire `<form name="contact" netlify>` fonctionnera automatiquement (onglet *Forms*).
4. Ajoutez votre domaine plus tard (Netlify → *Domain management*). SSL est auto.

**Déploiement via CLI**
```bash
npm i -g netlify-cli
netlify deploy --prod --dir=site
```

## Option B — GitHub Pages (gratuit)

1. Créez un dépôt `snapdish-site`, ajoutez le contenu du dossier **/site** à la racine du repo.
2. Réglages du repo → *Pages* → *Deploy from branch* (branche `main`, `/root`).
3. Votre site sera accessible à `https://<votre-user>.github.io/snapdish-site/`

## Option C — Vercel (simple, très rapide)

1. `vercel` (après `npm i -g vercel`) depuis le dossier **/site** ou connectez le repo GitHub.
2. Choisir *Other* / *Static HTML* quand Vercel demande le framework.

## Option D — Hébergeur classique (OVH/Infomaniak/IONOS)

1. Créez le domaine et l'hébergement mutualisé.
2. Uploadez le contenu de **/site** dans le dossier `www/` via FTP.
3. Activez le HTTPS/SSL dans le panneau de l'hébergeur.

## Option E — Intégration Odoo Website

- Recréez la structure via les *snippets* Odoo en copiant les textes/sections.
- Ajoutez un *code block* pour de petites touches CSS si besoin.
- Branchez le formulaire Odoo (Website → Form builder) vers le CRM pour capter les leads.
- Reprenez les couleurs: primaire `#C62828` et accent `#FFC233`.

## Remplacements conseillés

- Remplacez `assets/snapdish-logo-base.png` par votre logo final.
- Mettez à jour l'email/WhatsApp dans la section Contact.
- Ajoutez vos cas réels dans le bloc **Avant / Après**.

Bon déploiement !
