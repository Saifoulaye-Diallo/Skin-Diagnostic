Parfait Saifoulaye 🎯 Voici un **README complet** pour ton projet de diagnostic du cancer de la peau, fullstack avec **Django + React + Docker**, prêt à être déployé sur **Railway** :

---

## 🧪 Skin Diagnostic – Application Web de Détection du Cancer de la Peau

Application complète (frontend React + backend Django + PostgreSQL) permettant aux utilisateurs de soumettre des images de leur peau pour obtenir un **diagnostic automatique** grâce à un modèle d’intelligence artificielle.

---

### 🛠️ Technologies utilisées

- 🐍 Django / Django Rest Framework (API)
- ⚛️ React + TypeScript + TailwindCSS (Frontend)
- 🐘 PostgreSQL (Base de données)
- 🐳 Docker / Docker Compose
- ☁️ Déploiement Railway

---

## 📁 Structure du projet

```
.
├── docker-compose.yml           # Compose file pour prod (backend + frontend + db)
├── skin_diagnostic/             # App Django (backend)
│   ├── Dockerfile
│   ├── .env
│   └── ...
├── project0/                    # App React (frontend)
│   ├── Dockerfile
│   ├── nginx.conf
│   └── ...
```

---

## 🚀 Lancer le projet en local (dev)

```bash
docker-compose -f docker-compose.yml up --build
```

---

## 🌍 Déploiement sur Railway

> Railway est utilisé pour le déploiement Docker fullstack

### 1. 🧭 Étapes

- Pousse le projet sur GitHub
- Va sur https://railway.app
- "New Project" → "Deploy from GitHub Repo"
- Railway détecte `docker-compose.yml`
- Ajoute tes variables d’environnement (`.env`)
- Lance le build

---

### 2. 🔐 Variables d’environnement requises (backend)

```env
DJANGO_SECRET_KEY=your-secret-key
DEBUG=False
ALLOWED_HOSTS=railway.app, *.railway.app
POSTGRES_DB=skin_db
POSTGRES_USER=user
POSTGRES_PASSWORD=password
POSTGRES_HOST=db
POSTGRES_PORT=5432
```

---

## 👤 Fonctionnalités principales

- ✅ Authentification (inscription / connexion) avec JWT
- ✅ Formulaire d’envoi de diagnostic (nom, prénom, date de naissance, image)
- ✅ Affichage des diagnostics passés
- ✅ Gestion du thème clair/sombre 🌙
- ✅ Interface en **français**
- ✅ Animation fluide avec Framer Motion
- ✅ Mode production via NGINX (frontend)

---

## 📦 Commandes utiles

### Backend Django

```bash
docker exec -it django_backend bash
python manage.py migrate
python manage.py createsuperuser
```

### Frontend React (dev)

```bash
cd project0
npm install
npm run dev
```

---

## ✅ Crédits

Développé par **Saifoulaye Diallo**  
Projet académique/testé avec IA pour la détection de maladies cutanées

---

Souhaites-tu que je te le génère en fichier `README.md` directement ?
