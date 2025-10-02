# arnaudgoetz.github.io

Portfolio personnel d'Arnaud Goetz - Développeur Full Stack

🌐 **Site web :** [https://arnaudgoetz.github.io](https://arnaudgoetz.github.io)

## 📋 À propos

Ce site portfolio présente mon parcours professionnel, mes compétences, mes expériences et mes projets en développement informatique.

## 🗂️ Structure du site

- **Accueil** (`index.md`) - Présentation générale, compétences clés et liens rapides
- **Parcours scolaire** (`parcours.md`) - Formation académique, diplômes et certifications
- **Expériences professionnelles** (`experiences.md`) - Historique professionnel détaillé et compétences
- **Projets** (`projets.md`) - Portfolio de projets personnels et professionnels
- **Contact** (`contact.md`) - Informations de contact et formulaire

## 📁 Organisation des fichiers

```
arnaudgoetz.github.io/
├── index.md              # Page d'accueil
├── parcours.md           # Parcours scolaire
├── experiences.md        # Expériences professionnelles
├── projets.md            # Projets
├── contact.md            # Contact
├── _config.yml           # Configuration Jekyll
├── .gitignore            # Fichiers à ignorer
└── assets/
    ├── images/           # Images et logos
    │   └── README.md     # Instructions pour les images
    ├── documents/        # Documents téléchargeables (CV, diplômes, etc.)
    │   └── README.md     # Instructions pour les documents
    └── css/              # Styles personnalisés (optionnel)
```

## 🚀 Technologies utilisées

- **Jekyll** - Générateur de site statique
- **GitHub Pages** - Hébergement
- **Markdown** - Rédaction du contenu
- **Minima theme** - Thème Jekyll

## 📝 Comment ajouter du contenu

### Ajouter des images

1. Placez vos images dans le dossier `assets/images/`
2. Référencez-les dans les fichiers Markdown : `![Description](/assets/images/nom_fichier.jpg)`
3. Consultez `assets/images/README.md` pour la liste des images à ajouter

### Ajouter des documents

1. Placez vos documents PDF dans le dossier `assets/documents/`
2. Créez des liens dans les fichiers Markdown : `[Texte du lien](/assets/documents/nom_fichier.pdf)`
3. Consultez `assets/documents/README.md` pour la liste des documents à ajouter

### Modifier le contenu

Éditez simplement les fichiers `.md` correspondants et committez les changements. GitHub Pages recompilera automatiquement le site.

## 🛠️ Développement local

Pour tester le site en local :

```bash
# Installer Jekyll (nécessite Ruby)
gem install bundler jekyll

# Cloner le repository
git clone https://github.com/ArnaudGoetz/arnaudgoetz.github.io.git
cd arnaudgoetz.github.io

# Créer un Gemfile si nécessaire
bundle init
bundle add jekyll
bundle add minima

# Lancer le serveur local
bundle exec jekyll serve

# Ouvrir dans le navigateur
# http://localhost:4000
```

## 📦 Configuration

La configuration du site se trouve dans `_config.yml`. Vous pouvez y modifier :
- Le titre du site
- La description
- Les liens de navigation
- Le thème

## ✅ Checklist pour personnaliser le site

- [ ] Remplacer les informations de contact par les vraies
- [ ] Ajouter une vraie photo de profil (`assets/images/profile.jpg`)
- [ ] Ajouter le CV en PDF (`assets/documents/cv_arnaud_goetz.pdf`)
- [ ] Ajouter les logos des entreprises et écoles
- [ ] Ajouter les captures d'écran des projets
- [ ] Ajouter les documents de certifications
- [ ] Personnaliser les liens vers les réseaux sociaux
- [ ] Ajouter les liens GitHub vers les vrais projets
- [ ] Configurer un formulaire de contact fonctionnel
- [ ] Optimiser toutes les images pour le web

## 🎨 Personnalisation avancée

### Modifier le thème

Vous pouvez personnaliser l'apparence en :
1. Modifiant `_config.yml` pour changer de thème
2. Ajoutant des fichiers CSS personnalisés dans `assets/css/`
3. Créant des layouts personnalisés dans `_layouts/`

### Ajouter des pages

Créez un nouveau fichier `.md` avec le front matter approprié :

```markdown
---
layout: page
title: Titre de la page
permalink: /url-de-la-page/
---

Contenu de la page...
```

## 📄 Licence

Ce portfolio est à usage personnel. Tous droits réservés.

## 📞 Contact

Pour toute question : [arnaud.goetz@example.com](mailto:arnaud.goetz@example.com)

---

*Dernière mise à jour : Octobre 2024*
