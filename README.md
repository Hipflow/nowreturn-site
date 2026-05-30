# nowreturn.app

Site web minimaliste pour Return — Privacy Policy + Support.

## Pages

- `/` (index.html) — landing minimaliste
- `/privacy` (privacy.html) — Privacy Policy FR + EN
- `/support` (support.html) — FAQ + contact

## Hébergement : GitHub Pages

```bash
cd /Users/mathieumartin/Documents/Claude/nowreturn-site
git init
git add .
git commit -m "v1 — landing + privacy + support"
gh repo create hipflow/nowreturn-site --public --source=. --push
```

Puis dans GitHub :
- **Settings → Pages**
- **Source** : Deploy from a branch → `main` → `/(root)` → Save
- Attendre 1-2 min, le site est live sur `https://hipflow.github.io/nowreturn-site/`

## Custom domain (optionnel — si tu achètes nowreturn.app)

Le fichier `CNAME` contient déjà `nowreturn.app`. Une fois le domaine acheté :
1. DNS : ajoute un enregistrement CNAME `@ → hipflow.github.io`
2. GitHub Settings → Pages → Custom domain : `nowreturn.app` → Save
3. Coche "Enforce HTTPS"

## URLs pour App Store Connect

Sans custom domain :
- Privacy : `https://hipflow.github.io/nowreturn-site/privacy`
- Support : `https://hipflow.github.io/nowreturn-site/support`

Avec custom domain :
- Privacy : `https://nowreturn.app/privacy`
- Support : `https://nowreturn.app/support`
