# 🚀 MultimédiaTeams - Application de Gestion de Projets

## 📋 Description
MultimédiaTeams est une application web moderne de gestion de projets conçue spécifiquement pour les équipes d'étudiants. Elle permet de créer et gérer des projets, d'assigner des tâches, et de collaborer efficacement en équipe.

## ✨ Fonctionnalités principales
- 📊 Tableau de bord intuitif
- 📝 Gestion des tâches avec statuts (À faire, En cours, Terminé)
- 👥 Gestion des membres d'équipe
- 🔍 Système de recherche avancé
- 📱 Interface responsive

## 💻 Guide d'installation

### Prérequis
- Node.js (version 16.x ou supérieure)
- npm (version 8.x ou supérieure)
- Git
- Un navigateur web moderne

### Installation étape par étape

1. **Cloner le projet**
   ```bash
   # Cloner le dépôt
   git clone https://github.com/yosraessid/multim-diateamsweb.git
   
   # Accéder au répertoire
   cd multim-diateamsweb
   ```

2. **Installer les dépendances**
   ```bash
   # Installation avec npm
   npm install
   ```

3. **Configuration de l'environnement**
   ```bash
   # Créer le fichier .env
   cp .env.example .env
   ```
   
   Contenu minimal du fichier `.env` :
   ```env
   VITE_API_URL=http://localhost:3008
   VITE_APP_NAME=MultimédiaTeams
   ```

4. **Lancer l'application**
   ```bash
   # Mode développement
   npm run dev
   
   # L'application sera accessible sur :
   # http://localhost:3008
   ```

### Configuration avancée

#### Configuration du port
Si le port 3008 est déjà utilisé, modifiez le fichier `vite.config.js` :
```javascript
export default defineConfig({
  server: {
    port: 3008, // Changez ce numéro
    host: true
  }
})
```

#### Scripts disponibles
```bash
# Démarrer en mode développement
npm run dev

# Construire pour la production
npm run build

# Prévisualiser la version de production
npm run preview
```

## 🚀 Déploiement

### Build de production
```bash
# Créer une version optimisée
npm run build

# Les fichiers seront générés dans le dossier /dist
```

### Structure des fichiers de production
```
dist/
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
├── index.html
└── ...
```

## 🔧 Résolution des problèmes courants

### "Port already in use"
```bash
# Trouver le processus
lsof -i :3008

# Arrêter le processus
kill -9 [PID]
```

### Problèmes de dépendances
```bash
# Nettoyer le cache
npm cache clean --force

# Réinstaller les dépendances
rm -rf node_modules
npm install
```

## 📝 Bonnes pratiques

### Développement
1. Suivre les conventions de code
2. Commenter le code important
3. Utiliser les branches Git pour les nouvelles fonctionnalités
4. Faire des commits réguliers et descriptifs

### Sécurité
- Ne jamais commiter le fichier `.env`
- Maintenir les dépendances à jour
- Exécuter régulièrement `npm audit`
- Utiliser HTTPS en production

## 🛠️ Technologies utilisées
- React 18
- Vite
- React Router DOM
- Lucide Icons
- PropTypes

## 📱 Compatibilité
- ✅ Chrome (recommandé)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## 👥 Contribution
1. Fork le projet
2. Créer une branche
   ```bash
   git checkout -b feature/nouvelle-fonctionnalite
   ```
3. Commit les changements
   ```bash
   git commit -m "Ajout de la nouvelle fonctionnalité"
   ```
4. Push vers la branche
   ```bash
   git push origin feature/nouvelle-fonctionnalite
   ```
5. Ouvrir une Pull Request

## 🆘 Support

### Documentation
- [Documentation complète](https://github.com/yosraessid/multim-diateamsweb/wiki)
- [Guide de contribution](CONTRIBUTING.md)
- [Notes de version](CHANGELOG.md)

### Aide et contact
- Ouvrir une issue sur GitHub
- Contacter l'équipe de développement
- Consulter la FAQ dans le wiki

## 📄 Licence
Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 👤 Auteur
- Essid Yosra

---
Développé avec ❤️ par Essid Yosra
