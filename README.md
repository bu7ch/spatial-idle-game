```markdown
# 🚀 Idle Game Spatial (Version Rails)

Bienvenue dans le dépôt de la version **Ruby on Rails** d'un jeu idle à thème spatial.  
Ce projet est conçu comme un **support pédagogique** pour les développeurs juniors souhaitant apprendre Rails en contribuant à un jeu fonctionnel et évolutif.

Le jeu se déroule dans l'espace : vous gérez une base, collectez du **Deterhium** (ressource principale) grâce à des robots, achetez des améliorations, et pouvez même faire des **prestiges** pour obtenir des bonus permanents. Plus tard, des interactions sociales (classements) viendront enrichir l'expérience.

> **Deux versions sont prévues** : une première en Rails (ce dépôt), puis une seconde en Laravel, afin de comparer les approches et d'apprendre deux frameworks populaires.

---

## 🎯 Objectifs pédagogiques

- Découvrir Rails 8 avec **Hotwire** (Turbo + Stimulus) pour une expérience SPA sans framework JavaScript lourd.
- Mettre en pratique les concepts clés : MVC, ORM (ActiveRecord), migrations, jobs asynchrones (GoodJob), tests (RSpec), déploiement.
- Comprendre la logique métier d'un jeu idle (gestion de ressources, générateurs, upgrades, prestige).
- Apprendre à contribuer à un projet open source via des issues cadrées et des pull requests.

---

## 🧰 Stack technique

- **Ruby 3.4+** / **Rails 8+**
- **PostgreSQL** (base de données)
- **Hotwire** (Turbo + Stimulus) pour les mises à jour dynamiques
- **Tailwind CSS** pour le style
- **Devise** pour l'authentification
- **GoodJob** pour les tâches asynchrones
- **RSpec** pour les tests (à venir)
- **Déploiement** : Render (ou autre)

---

## 🚀 Installation en local

### Prérequis

- Ruby 3.4 ou supérieur
- PostgreSQL installé et démarré (voir [comment démarrer PostgreSQL](#postgresql))
- Git
- Node.js et Yarn (pour Tailwind)

### Étapes

1. **Cloner le dépôt**
   ```bash
   git clone https://github.com/votre-utilisateur/idle-game-rails.git
   cd idle-game-rails
   ```

2. **Installer les dépendances Ruby**
   ```bash
   bundle install
   ```

3. **Configurer la base de données**
   - Copier le fichier `config/database.yml.example` en `config/database.yml` (si existant) ou adapter les identifiants PostgreSQL.
   - Créer la base de données :
     ```bash
     rails db:create
     rails db:migrate
     ```

4. **Installer les dépendances JavaScript** (pour Tailwind)
   ```bash
   yarn install
   ```

5. **Lancer le serveur**
   ```bash
   rails server
   ```
   Rendez-vous sur `http://localhost:3000`.

### PostgreSQL

Si vous rencontrez l'erreur `ActiveRecord::ConnectionNotEstablished`, vérifiez que PostgreSQL est démarré :

- **macOS (Homebrew)** : `brew services start postgresql`
- **Linux (systemd)** : `sudo systemctl start postgresql`
- **Windows** : démarrez le service via le gestionnaire de services.

---

## ☁️ Déploiement

Le projet est configuré pour être déployé sur **Render** facilement.  
Consultez le fichier `render.yaml` pour la configuration.  
Après avoir lié votre dépôt à Render, le déploiement se fera automatiquement à chaque push sur `main`.

---

## 🤝 Contribuer

Ce projet vit grâce aux contributions de juniors comme vous !  
Nous avons structuré le développement en **phases** claires, chaque phase étant découpée en **issues** avec des labels `good first issue` pour vous guider.

### Comment contribuer ?

1. Lisez le [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
2. Consultez le [CONTRIBUTING.md](CONTRIBUTING.md) pour les règles de contribution.
3. Parcourez les [issues](https://github.com/votre-utilisateur/idle-game-rails/issues) et choisissez-en une.
4. Commentez l'issue pour signaler que vous vous en chargez.
5. Suivez les instructions dans l'issue, faites une pull request.

### Roadmap

Le développement suit les phases suivantes (consultez le [Projet GitHub](https://github.com/votre-utilisateur/idle-game-rails/projects) pour l'avancement) :

- **Phase 0** : Initialisation du projet (Rails + Devise + déploiement)
- **Phase 1** : Ressource unique et clic manuel
- **Phase 2** : Premier robot collecteur
- **Phase 3** : Multiples ressources
- **Phase 4** : Améliorations (upgrades)
- **Phase 5** : Système de prestige
- **Phase 6** : Interactions sociales (classements)
- **Phase 7** : Tests, UI/UX et documentation pour Laravel

---

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE).

---

## 🙏 Remerciements

Merci à tous les contributeurs, débutants ou confirmés, qui donnent vie à ce jeu pédagogique.  
N'hésitez pas à poser des questions dans les issues ou à nous contacter.

**Bon code et bon jeu !** 👨‍🚀👩‍🚀
```