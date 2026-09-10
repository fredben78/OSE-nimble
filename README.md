# Dolmenwood sous Nimble

Conversion communautaire, non-officielle, du cadre de campagne *Dolmenwood* (Necrotic Gnome) vers le système *Nimble* (Nimble Co.).

Site publié via GitHub Pages, généré avec [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

## Contenu

- **Règles** : création de personnage, sorts (Magicien/Clerc), fondamentaux Nimble
- **Bestiaire** : 158 créatures converties depuis le Dolmenwood Monster Book

Voir [NOTICE.md](docs/NOTICE.md) pour les mentions légales et l'attribution.

## Développement local

```bash
pip install -r requirements.txt
mkdocs serve
```

Puis ouvrir http://127.0.0.1:8000.

## Déploiement

Le déploiement sur GitHub Pages est automatique à chaque push sur `main` (voir `.github/workflows/deploy.yml`). Il construit le site et le publie sur la branche `gh-pages`.

**Première configuration** (une seule fois) : dans les paramètres du dépôt GitHub, section *Pages*, choisir la source *Deploy from a branch* → branche `gh-pages` → dossier `/ (root)`.
