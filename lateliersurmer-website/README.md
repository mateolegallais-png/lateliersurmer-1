# L'Atelier sur Mer — Site Web

Site web statique de **L'Atelier sur Mer**, expert en décoration de voile, covering nautique et supports publicitaires depuis 2003. Basé à La Trinité-sur-Mer et Lorient, Bretagne.

## 🌐 URL GitHub Pages

> **https://[votre-organisation].github.io/[nom-du-repo]/**
>
> *(Remplacer par l'URL réelle après déploiement)*

## 📄 Pages

| Fichier | Page |
|---|---|
| `index.html` | Accueil |
| `about.html` | Qui sommes-nous |
| `expertise.html` | Notre Savoir-Faire |
| `course-au-large.html` | Course au Large |
| `yachting.html` | Yachting |
| `sail-decoration.html` | Décoration sur voile |
| `covering.html` | Covering |
| `advertising.html` | Supports publicitaires |
| `gallery.html` | Nos Réalisations |
| `mentions-legales.html` | Mentions légales |
| `politique-de-confidentialite.html` | Politique de confidentialité |
| `gestion-des-cookies.html` | Gestion des cookies |
| `404.html` | Page introuvable |

## 🛠️ Déploiement GitHub Pages

1. Créer un dépôt GitHub (public ou privé avec GitHub Pro)
2. Pousser tous les fichiers à la racine du dépôt
3. Dans **Settings → Pages** : source = `main` branch, dossier `/root`
4. Le fichier `.nojekyll` est déjà présent pour désactiver Jekyll

## 📧 Configuration EmailJS (formulaire de contact)

Le formulaire de contact utilise [EmailJS](https://www.emailjs.com/). Pour l'activer :

1. Créer un compte sur emailjs.com
2. Créer un **Service** (Gmail, SMTP, etc.) → noter le `Service ID`
3. Créer un **Template** avec les variables : `from_name`, `from_email`, `company`, `phone`, `message` → noter le `Template ID`
4. Copier la **Public Key** depuis Account → API Keys
5. Dans `index.html`, remplacer les 3 valeurs suivantes :

```js
const EMAILJS_SERVICE_ID  = 'YOUR_SERVICE_ID';   // ex: 'service_abc123'
const EMAILJS_TEMPLATE_ID = 'YOUR_TEMPLATE_ID';  // ex: 'template_xyz789'
const EMAILJS_PUBLIC_KEY  = 'YOUR_PUBLIC_KEY';   // ex: 'AbCdEfGhIjKlMnOp'
```

## 📝 Informations à compléter

Dans `mentions-legales.html`, les champs suivants sont marqués `[à compléter]` :
- Forme juridique de la société
- Nom du directeur de publication
- Hébergeur du site (nom, adresse, téléphone)

## 🖼️ Images

Toutes les images sont stockées localement dans `images/` (42 fichiers).
Logo principal : `images/assets/logo_asm.png`

## 🌍 Langues

Bilingue FR/EN — bascule via le bouton langue dans la barre de navigation.
La préférence est sauvegardée dans `localStorage` (clé : `asm_lang`).

---

© 2025 L'Atelier sur Mer
