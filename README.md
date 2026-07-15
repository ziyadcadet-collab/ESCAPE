# ✈️ CLEAR TO PUSH — Escape Game Sécurité Piste

Serious game de sensibilisation terrain (prévention TMS & sécurité poste avion) — Alyzia QSE.

## Principe
Le vol AZ 4521 doit partir dans 6 minutes. Les opérateurs explorent la **photo aérienne du poste K12**
pour détecter **10 risques** (opérationnels et TMS), puis valident la **bonne action corrective**
pour lever chaque obstacle. Tous les obstacles levés → l'avion part.

## Anti-mémorisation
Les **10 risques sont tirés au sort à chaque partie** dans une banque de **16 scénarios**
(+ leurres « conformes » eux aussi variables). Impossible d'apprendre le poste par cœur : il faut
réellement observer. L'ordre des réponses est également mélangé à chaque ouverture de fiche.

## Utilisation
- Deux fichiers seulement : `index.html` + l'image `assets/apron.jpg`. Aucune API, aucune installation,
  aucune dépendance JS ; fonctionne hors-ligne une fois les fichiers récupérés.
- Fonctionne sur PC, tablette et mobile (navigateur récent).
- Idéal en causerie sécurité, quart d'heure sécurité, journée SST.
- **Tour d'inspection guidé** : fond photographique aérien du poste ; des **pastilles**
  marquent chaque zone à inspecter (le survol affiche son nom : GPU, camion avitailleur, escalier…).
  On clique, on identifie le risque et on choisit la bonne action — ou on confirme la conformité.
  Effet « CLEAR TO PUSH » à la fin.
- **Deux modes** (choisis au démarrage) :
  - **Sensibilisation** — zones *visibles*, 6:00, pour le grand public (causerie, quart d'heure sécurité) ;
  - **Détection** — zones *cachées, révélées au survol*, 4:00, avec compteur « zones inspectées »,
    pour entraîner la **vigilance** d'un public déjà sensibilisé.
- **Meilleur score** conservé localement (localStorage) d'une partie à l'autre.
- **Accessible** : navigation clavier (Tab + Entrée/Espace), fermeture d'une fiche risque par Échap,
  respect de `prefers-reduced-motion`.

## Mécanique de jeu
| Action | Points |
|---|---|
| Bonne action corrective | +100 |
| Zone conforme vérifiée (RAS) | +10 |
| Mauvaise action corrective | −30 |
| Indice | −50 |
| Bonus | temps restant ÷ 2 |

## Image de fond
`assets/apron.jpg` est une image **générée par IA** (originale, sans droits de tiers). Pour changer
de décor, remplacez ce fichier par une autre vue aérienne au même cadrage (~3:2) ; les positions des
risques sont exprimées en pourcentages dans `index.html` et se réajustent facilement.

## Déploiement
Hébergé via GitHub Pages — voir la section Pages des paramètres du dépôt.

---
Réalisé pour la prévention des TMS — Direction QSE/SST.
