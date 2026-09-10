# Fondamentaux Nimble

Aide-mémoire des règles Nimble telles quelles (pas d'adaptation Dolmenwood ici — pour ça, voir [Création de personnage](creation-personnage.md) et [Sorts](sorts.md)).

## Résolution des attaques

Pas de jet d'attaque séparé : lancez directement le(s) dé(s) de dégâts.

- Un **1 sur le dé principal** (le plus à gauche s'il y en a plusieurs) = raté total, aucun dégât.
- Le **maximum sur le dé principal** = critique : relancez-le et ajoutez au total (répétable à l'infini).
- Attaques multiples au même tour : chaque attaque après la première subit un désavantage cumulatif.
- Les critiques ignorent l'armure des monstres.

## Armure

- **Héros** : l'armure ne réduit rien passivement. Elle s'applique uniquement via la réaction **Défendre** (1×/round), qui soustrait votre Armure aux dégâts d'une attaque.
- **Monstres** : armure passive et permanente. Armure Moyenne = somme des dés de dégâts seulement (ignore les modificateurs). Armure Lourde = moitié de la somme des dés (arrondi au supérieur, ignore les modificateurs).

## Points de vie, Blessures, mort

- À 0 PV : gagnez 1 Blessure + état Mourant jusqu'à regagner des PV.
- Mort à 6 Blessures.
- En état Mourant : actions limitées à 1, Concentration rompue. Attaquer/lancer un sort inflige 1 Blessure sauf réussite d'un JdS FOR (DC 10). Subir des dégâts inflige 2 Blessures (3 sur un critique).

## Magie — Mana et rangs

- Coût d'un sort = son rang. Les cantrips (sorts mineurs) sont gratuits.
- Amplification (upcast) : possible jusqu'au rang débloqué par le lanceur, en dépensant plus de Mana.
- Une seule Concentration active à la fois ; rompue par un JdS FOR raté suite à des dégâts critiques.
- Lancer un sort nécessite une main libre (ou un focus tenu) et la capacité de parler.
- **Portée (Range) vs Contact (Reach)** : un sort à Portée est lancé avec désavantage si un ennemi est adjacent au lanceur ; un sort à Contact n'a pas cette pénalité.
- Les effets de zone (AoE) ne ratent ni ne critiquent jamais ; un seul jet s'applique à toutes les cibles.

## Seuils de Difficulté (SD) — tests de compétence

| Difficulté | SD | Exemple |
|---|---|---|
| Facile | 8 | Repérer un ogre mal caché |
| Moyen | 12 | Trouver une porte secrète |
| Difficile | 15 | Calmer une bête blessée et prise au piège |
| Très difficile | 18 | Percer les intentions d'un espion aguerri |
| Extrême | 20+ | Désamorcer un piège ancien et légendaire |

Plafond d'une compétence : **+12**.

## DC des jets de sauvegarde imposés

- **Par une capacité de héros** (sort, trait, capacité de classe) : **10 + stat clé du lanceur**.
- **Par un monstre** : suit une table liée à son niveau (chaque créature convertie du Bestiaire précise déjà son propre DC) :

| Niveau monstre | 1/4-1/3 | 1/2-1 | 2-3 | 4-5 | 6-7 | 8-9 | 10-11 | 12-13 | 14-15 | 16-17 | 18-20 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| DC | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19-20 |

## Avantage / Désavantage

Pas « 2d20, garder un résultat » : on **ajoute un dé du même type** au jet et on retire le plus bas (avantage) ou le plus haut (désavantage). Sur un jet d20 simple, le résultat revient au même que sur d'autres systèmes ; le même principe s'applique aussi aux dés de dégâts (avantage sur les dégâts = ajouter un dé et retirer le plus bas).

## Repères de calibrage (pour toute création homebrew)

- Un bonus fixe permanent sur une Ascendance ne dépasse normalement pas **+1** ; au-delà, préférez une capacité à charges (1×/repos sûr, 1×/rencontre).
- Le **dé de base d'une arme ou d'un sort ne grossit jamais** avec le niveau. En revanche, plusieurs classes ont un **dé de ressource dédié** qui grossit explicitement par palier de niveau — ce n'est pas une exception à la règle précédente, c'est un mécanisme de classe séparé. Exemples : Dés de Fureur du Berserker (1d4 → d6 → d8 → d10 → d12), Dés de Combat du Commandant (d8 → d10 → d12 → d20), Attaque Sournoise du Tricheur (1d6 → 1d8 → 2d8 → 2d10 → 2d12 → 2d20 → 3d20), Dés de Jugement du Chevalier du Serment (d8 → d10 → d12 → d20).
- Coût en actions d'un sort : cantrip/réaction/effet simple non-dommageable = **1 action** ; sort de rang normal = **2 actions** ; grand sort de zone à distance = **3 actions**. Un sort de rang 1 typique fait environ **3 dés** de dégâts pour 2 actions (ex. *Magic Missile* : 2 actions, 1d4+1 ×3, ne rate jamais).
- Les effets qui **ignorent l'armure** sont un marqueur de puissance fort — à réserver aux sorts qui n'ont rien d'autre en plus.

## Correspondances rapides depuis un système à d20 ascendant (5e-like)

| Concept | Équivalent Nimble |
|---|---|
| JdS Constitution | JdS FOR |
| JdS Sagesse / Charisme | JdS VOL |
| Compétence Athlétisme | Force *(Might)* |
| Compétence Escamotage/Acrobaties | Finesse |
| Compétence Dressage/Nature/Survie | Survie *(Naturecraft)* |
| Compétence Tromperie/Persuasion/Représentation | Influence |
| Compétence Histoire/Religion | Savoir *(Lore)* |
| Compétence Investigation/Médecine | Investigation *(Examination)* |
| États Paralysé/Étourdi/Inconscient | Incapacité |
| CA 14-17 (monstre) | Armure Moyenne |
| CA <14 (monstre) | Sans armure |
| CA >17 (monstre) | Armure Lourde |

*Note : Discrétion (Stealth) et Perception existent déjà telles quelles comme compétences Nimble — pas de conversion nécessaire pour elles.*
