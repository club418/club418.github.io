# CLUB 418

Site officiel de l'association CLUB 418, pour la promotion du numérique citoyen à Poitiers.


## Installation locale

### Option 1 : Avec Docker Compose

#### Prérequis
- [Docker](https://www.docker.com/get-started) et [Docker Compose](https://docs.docker.com/compose/install/) installés

#### Configuration

Un fichier `compose.yml` est déjà présent à la racine du projet.

#### Commandes

```bash
# Démarrer le serveur
docker compose up

# Démarrer en arrière-plan
docker compose up -d

# Voir les logs
docker compose logs -f

# Arrêter le serveur
docker compose down
```

**Note** :

- La configuration de développement (`_config_dev.yml`) est automatiquement chargée avec Docker Compose

Le site sera accessible sur **http://localhost:4000**

#### Rebuild du site

```bash
# Reconstruire le site si vous modifiez les dépendances
docker compose down
docker compose up --build
```


### Option 2 : Installation classique Ruby/Jekyll

#### Prérequis

- **Ruby** >= 3.0 ([Installation Ruby](https://www.ruby-lang.org/fr/documentation/installation/))
- **Bundler** (`gem install bundler`)
- **Git**

#### Installation et lancement

**TODO**


