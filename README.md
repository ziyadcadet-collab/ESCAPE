# ✈️ CLEAR TO PUSH — Escape Game Sécurité Piste

Serious game de sensibilisation terrain (prévention TMS & sécurité poste avion) — Alyzia QSE.

## Principe
Le vol AZ 4521 doit partir dans 6 minutes. Les opérateurs cliquent sur la carte du poste K12
pour détecter **10 risques** (opérationnels et TMS), puis valident la **bonne action corrective**
pour lever chaque obstacle. Tous les obstacles levés → l'avion part.

## Utilisation
- 100 % autonome : un seul fichier `index.html`, aucune API, aucune installation.
- Fonctionne sur PC, tablette et mobile (navigateur récent).
- Idéal en causerie sécurité, quart d'heure sécurité, journée SST.

## Mécanique de jeu
| Action | Points |
|---|---|
| Obstacle levé (bonne action) | +100 |
| Mauvaise action corrective | −30 |
| Fausse alerte (élément conforme) | −20 |
| Clic dans le vide | −10 |
| Indice | −50 |
| Bonus | temps restant ÷ 2 |

## Déploiement
Hébergé via GitHub Pages — voir la section Pages des paramètres du dépôt.

---
Réalisé pour la prévention des TMS — Direction QSE/SST.
