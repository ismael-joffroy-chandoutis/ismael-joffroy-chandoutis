# Maintenance — liste des apps Pinokio validées

Système conçu pour être piloté depuis **n'importe quel client Claude** (web, mobile,
desktop, CLI), sans recoller de prompt.

## Les 3 façons de mettre à jour

### 1. Manuel, depuis le mobile/web — `/pinokio-update` ⭐ recommandé
Ouvre Claude (app mobile, claude.com/code, desktop ou CLI) sur le repo
`12georgiadis/12georgiadis` et tape :

```
/pinokio-update
```

La commande fait tout : recherche → édition de `pinokio-validated-apps.md` → commit →
push → PR avec résumé. Variante sans PR : `/pinokio-update --no-pr`.

> Le playbook est versionné dans [`.claude/commands/pinokio-update.md`](.claude/commands/pinokio-update.md),
> donc il est identique sur tous tes appareils et évolue avec le repo.

### 2. Planifié, sans intervention — trigger Claude Code on web
Dans les réglages de ton environnement Claude Code on web, crée un **trigger planifié** :
- **Schedule (cron)** : ex. `0 9 * * 1` (lundi 9h).
- **Branche** : `claude/pinokio-validated-apps-W6RgH` (ou `main` après merge).
- **Network policy** : accès sortant autorisé (github.com, pinokio.co, beta.pinokio.co).
- **Prompt** : `/pinokio-update`

À chaque exécution, une session démarre seule, met à jour et ouvre une PR à relire.
Doc : https://code.claude.com/docs/en/claude-code-on-the-web

### 3. À la demande, en langage naturel
Dis simplement « refais une passe sur la liste Pinokio » dans une session — l'agent
chargera le même playbook.

## Architecture du système

| Fichier | Rôle |
|---|---|
| `pinokio-validated-apps.md` | **Le livrable** — la liste curatée (lisible par tous). |
| `.claude/commands/pinokio-update.md` | **Le moteur** — playbook de mise à jour, déclenché par `/pinokio-update`. |
| `MAINTENANCE.md` | Ce fichier — comment opérer le système. |

## Sources de vérité (rappel)
- **Vérifié** = org [`pinokiofactory`](https://github.com/orgs/pinokiofactory/repositories?type=all&sort=stargazers).
- **Communauté de confiance** = publishers identifiés/actifs ([beta.pinokio.co](https://beta.pinokio.co/) + Discord Pinokio).
- Règle d'or : vérifié **OU** acteur fiable identifié. Rien d'anonyme/non audité.
