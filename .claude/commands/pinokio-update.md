---
description: Met à jour pinokio-validated-apps.md (apps Pinokio validées + acteurs fiables) puis commit/push et ouvre/maj une PR.
argument-hint: "[--no-pr] (optionnel : met à jour le fichier sans ouvrir de PR)"
---

# Mise à jour de la liste des apps Pinokio validées

Tu maintiens le fichier `pinokio-validated-apps.md` à la racine du repo.
Exécute ce playbook de bout en bout, de façon autonome (aucun contexte préalable requis).

## 0. Préparation
- Branche de travail : `claude/pinokio-validated-apps-W6RgH`. Crée-la / bascule dessus
  (sinon développe sur la branche courante si elle a déjà été mergée dans `main`).
- Lis `pinokio-validated-apps.md` pour connaître l'état actuel (tableaux, acteurs, date).

## 1. Rafraîchir les apps VÉRIFIÉES (source de vérité)
- Scanne `https://github.com/orgs/pinokiofactory/repositories?type=all&sort=stargazers`.
- Relève chaque repo pertinent : nom, description, ⭐ actuel.
- Tout ce qui est dans `pinokiofactory` = **vérifié** (approuvé par Cocktail Peanut).
- Mets à jour les ⭐ et ajoute les nouveaux repos dans la bonne catégorie
  (Image / Vidéo / Audio-TTS / 3D / LLM-dev).

## 2. Rafraîchir les apps COMMUNAUTÉ de confiance
Pour chaque acteur fiable listé dans le fichier, vérifie ses nouvelles publications :
- **Cocktail Peanut** — `https://github.com/cocktailpeanut` + page d'accueil `https://beta.pinokio.co/`
- **Morpheus** — `https://beta.pinokio.co/u/morpheus`
- **PierrunoYT** — `https://github.com/PierrunoYT`
- **mrbizarro**, **IAnMove**, et les récurrents (holandeb, gujjubhai, dimz, clawt,
  theinaog, digifxron, krynsky) via `https://beta.pinokio.co/`.

## 3. Repérer de nouveaux acteurs fiables
- Sur `https://beta.pinokio.co/` (page d'accueil + apps en vedette), note tout publisher
  qui revient avec plusieurs apps qui fonctionnent.
- **Critère d'ajout d'un acteur** : plusieurs publications, activité récente, présence
  communautaire (Discord Pinokio). En cas de doute → ne pas ajouter, ou marquer « à vérifier ».

## 4. Règles d'inclusion (NE PAS dévier)
- ✅ Inclure si : dans `pinokiofactory` (vérifié) **OU** publisher identifié + actif + fiable.
- ❌ Exclure si : script anonyme / one-shot non audité → reste « community, à vos risques ».
- Conserver le ton honnête : les ⭐ sont indicatifs, et il n'existe pas de classement
  officiel « fiabilité » chez Pinokio (la seule garantie officielle = `pinokiofactory`).

## 5. Éditer le fichier
- Mets à jour les tableaux et la table des acteurs.
- Change la ligne **« Dernière mise à jour : YYYY-MM-DD »** avec la date du jour.
- Si des apps ont disparu de `pinokiofactory`, retire-les (elles ont été dévalidées).

## 6. Commit / push / PR
- Commit clair : `docs: refresh Pinokio validated apps list (YYYY-MM-DD)`.
- Push sur la branche (`git push -u origin <branche>`, retry avec backoff si réseau).
- Sauf si l'argument `--no-pr` est passé : ouvre une PR (ou pousse sur la PR existante)
  vers `main` avec un **résumé des changements** (apps ajoutées/retirées, acteurs ajoutés,
  ⭐ notables). Si une PR de cette branche est déjà ouverte, ne pas en créer une seconde.

## 7. Rapport final
Termine par un résumé court à l'écran : N apps vérifiées, N apps communauté, acteurs suivis,
ce qui a changé depuis la dernière passe, et le lien de la PR.
