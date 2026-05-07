# MADLORDS Magazine

Site Hugo bilingue FR/EN pour le magazine editorial de MADLORDS, joaillier specialise dans les pieces d'exception.

- **Site en ligne** : https://mag.madlords.com/
- **Repo** : analytics-ds/madlords
- **Stack** : Hugo (statique), GitHub Pages, GitHub Actions
- **Theme** : `mad-lords` (charte luxe, Playfair Display + DM Sans, palette noir/dore)
- **Langues** : Francais (par defaut, racine `/`), Anglais (`/en/`)

## Structure

- `content/` : articles et pages en francais
- `content/en/` : versions anglaises
- `themes/mad-lords/` : theme custom (layouts + CSS)
- `data/authors.yaml` : auteurs partages du reseau datashake (6 personas)
- `static/` : images, robots.txt, llms.txt, favicon, CNAME
- `.github/workflows/hugo.yml` : deploiement automatique sur GitHub Pages
- `.claude/` : skills et templates pour la generation de contenu via Claude Code

## Commandes locales

| Commande | Description |
|---|---|
| `/create-article-geo` | Creer un nouvel article (interactive, FR + EN, fetch image automatique) |
| `/seo` | Mode interactif SEO (meta tags, JSON-LD, audit on-page) |
| `/serve` | Lancer le serveur Hugo en local (http://localhost:1313/) |
| `/share` | Lancer Hugo + ngrok pour partager le site via un lien public |
| `/github-deploy` | Pull, commit et push vers GitHub Pages |

## Deploiement

Tout push sur `main` declenche automatiquement le build Hugo via GitHub Actions et le deploiement sur GitHub Pages (1-2 minutes).

## Contexte editorial

- Categories : Joaillerie, Maison, Art de vivre, Inspirations
- Auteur principal : magalie-ergoz (mode/beaute), claire-beaumont (maison)
- Ton : impersonnel, raffine, narratif
- Cible : amateurs de haute joaillerie, art de vivre premium
- Bilingue obligatoire : tous les articles sont publies en FR + EN avec un `translationKey` partage

## Equipe

Blog gere par Valentin et Jerome (consultants datashake). Voir le `CONTEXTE.md` du PBN GEO datashake (`100 Areas/Site web/`) pour le contexte global du reseau.
