# Convertir un jeu OSE vers Nimble — méthode

Une méthode générique pour porter un jeu de type OSE/B-X (D&D old-school, résolution d20 descendante ou ascendante, jets de compétence en d6, sauvegardes nommées) vers le système *Nimble*. Développée en convertissant un setting complet ; aucun élément spécifique à ce setting n'apparaît ici — seulement la technique.

## 1. Ce qui change fondamentalement

| OSE | Nimble |
|---|---|
| Jet d'attaque d20 vs CA | Aucun jet d'attaque : on lance directement les dés de dégâts. Un 1 sur le **dé principal** (le plus à gauche) = raté. Le maximum sur le dé principal = critique explosif (relance et cumul, sans limite). |
| Jet de compétence en d6 (ex. 2-en-6) ou d100 | Test de compétence d20 + bonus vs Seuil de Difficulté (SD 8/12/15/18/20+). |
| CA descendante ou ascendante | Armure Nimble : héros = DEX (+ bonus d'équipement), appliquée uniquement via la réaction **Défendre** (1×/round). Monstres : Armure passive fixe (Aucune/Moyenne/Lourde). |
| 5 sauvegardes nommées (Mort/Poison, Baguettes, Paralysie, Souffle, Sorts — ou leurs variantes narratives) | 4 stats seulement (FOR/DEX/INT/VOL) : Mort/Poison→FOR, Baguettes→DEX, Paralysie→FOR ou VOL selon l'effet, Souffle→DEX, Sorts→VOL ou INT selon l'effet (charme/domination→VOL, illusion→INT). |
| XP et niveaux individuels | Optionnel : ce projet a choisi la progression par paliers (le MJ décide quand le groupe monte de niveau), pour désamorcer le comptage d'XP — pas une règle Nimble, un choix de conversion. |

La résolution unifiée (tout passe par d20+bonus vs SD) est ce qui simplifie le plus : plus d'exception de dé selon le type de test.

## 2. Convertir un monstre

**L'astuce qui rend ça mécanique plutôt qu'arbitraire** : la plupart des jeux OSE ont un champ "Niveau" ou "Dés de Vie" qui joue le même rôle que le "Niveau de monstre" du Monster Builder Nimble — un monstre de Niveau N est calibré comme un défi pour un groupe de Niveau N, dans les deux systèmes. **Réutilisez ce nombre directement** comme clé d'entrée dans la table Nimble ci-dessous, sans formule de conversion à inventer :

| Niveau | PV (Sans armure) | PV (Armure M) | PV (Armure H) | Dégâts/round | Save DC |
|---|---|---|---|---|---|
| 1/4 | 12 | 9 | 7 | 3 | 9 |
| 1/2 | 18 | 15 | 11 | 7 | 10 |
| 1 | 26 | 20 | 16 | 11 | 10 |
| 2 | 34 | 27 | 20 | 13 | 11 |
| 3 | 41 | 33 | 25 | 15 | 11 |
| 4 | 49 | 39 | 29 | 18 | 12 |
| 5 | 58 | 46 | 35 | 19 | 12 |
| 6 | 68 | 54 | 41 | 21 | 13 |
| 8 | 91 | 73 | 55 | 26 | 14 |
| 10 | 118 | 94 | 71 | 30 | 15 |
| 12 | 149 | 119 | 89 | 35 | 16 |
| 15 | 203 | 162 | 122 | 43 | 17 |
| 18 | 266 | 213 | 160 | 52 | 19 |
| 20 | 313 | 250 | 189 | 54 | 20 |

**Armure** : si la CA source est déjà ascendante (échelle proche du d20, comme la 5e), le seuil officiel de conversion Nimble s'applique tel quel : CA 14-17 → Armure Moyenne, moins → Sans armure, plus → Armure Lourde. Si la CA source est descendante (B/X classique, CA 9 = pas d'armure), convertissez-la d'abord en CA ascendante (CA ascendante ≈ 19 − CA descendante) avant d'appliquer le seuil.

**Taille du dé de dégâts**, à choisir selon le thème de la créature, pas une règle stricte : d4 mort-vivant lent à gros bonus fixe, d6 humanoïde chaotique/petit, d8 mortel standard (défaut), d10 bête/animal, d12 géant/construct massif, d20 entité cosmique/dragon majeur.

**Capacités spéciales** : chaque capacité non-triviale ajoutée à un monstre de base doit faire baisser d'un cran sa ligne de PV/dégâts dans la table (ou traiter le monstre comme 1 niveau plus fort) — sinon on cumule gratuitement puissance de base et capacité bonus.

**Groupes nombreux et faibles → Minions** : plutôt que de forcer chaque individu d'un groupe faible dans la table ci-dessus (ce qui donne des PV ridiculement bas comparés à la table), utilisez la règle Minion de Nimble : pas de PV à suivre, toute attaque en tue un, dégâts combinés si plusieurs attaquent la même cible, pas de critique.

**Boss unique et nommé → Legendary** : une créature solo avec son propre lore (pas un "type" rencontré en groupe) est le cas d'usage du Legendary Monster Builder — elle agit après chaque tour de héros plutôt qu'une fois par round, avec des paliers Bloodied/Last Stand. Calibrez sur le **niveau du groupe de joueurs**, pas sur le niveau isolé du monstre.

## 3. Convertir des sorts et capacités

Trois catégories, pour ne pas réinventer ce qui existe déjà :

- **A — équivalent Nimble quasi-parfait** : reprenez le sort officiel existant, reflavoré. Zéro nouveau design, donc zéro risque de déséquilibre.
- **B — effet hors-combat, faible enjeu tactique** : convertissez en effet gratuit type Rituel (pas de Mana, non utilisable en combat sauf mention contraire).
- **C — effet puissant/narratif sans équivalent** : c'est le seul cas qui demande un vrai design. Calibrez sur les patrons confirmés :
  - Coût en actions : cantrip/réaction/effet simple = 1 action ; sort de rang normal = 2 actions ; grand sort de zone à distance = 3 actions.
  - Un sort de rang 1 typique fait environ 3 dés de dégâts pour 2 actions.
  - Les effets qui **ignorent l'armure** sont un marqueur de puissance fort à réserver aux sorts qui n'ont rien d'autre en plus.
  - DC de tout jet de sauvegarde imposé = **10 + stat clé du lanceur**.

## 4. Convertir des classes et des races/ascendances

- **Cherchez d'abord une classe Nimble existante** qui correspond à l'archétype avant d'en créer une nouvelle — Nimble a 11 classes de base (Berserker, Cheat, Commander, Hunter, Mage, Oathsworn, Shadowmancer, Shepherd, Songweaver, Stormshifter, Zephyr) qui couvrent large. Ne créez une classe entièrement neuve que si aucune ne colle, même en reflavorant.
- **Budget d'une Ascendance/race** : un bonus fixe permanent ne dépasse normalement pas **+1** ; au-delà, préférez une capacité à charges (1×/repos sûr, 1×/rencontre) plutôt qu'un bonus passif plus élevé.
- **Le dé de base d'une arme ou d'un sort ne grossit jamais avec le niveau.** Seules certaines classes ont un **dé de ressource dédié** qui grossit explicitement par palier (c'est un mécanisme de classe séparé, pas une exception générale) — n'accordez pas cette progression à une race/ascendance.

## 5. Pièges rencontrés en pratique

- **Gardez toujours le livre Nimble ouvert à côté, même pour un sort "repris tel quel".** C'est là que se cachent les erreurs les plus sournoises : un effet de base confondu avec son bonus d'amplification, une mécanique de jet de sauvegarde mal recopiée — des détails qui passent facilement inaperçus si on fait confiance à un premier jet familier plutôt que de relire le texte exact.
- **Sur un gros morceau de contenu (tout un bestiaire, une liste de sorts complète), prévoyez une relecture de cohérence dédiée**, séparée du travail de conversion lui-même : la terminologie dérive facilement d'une fiche à l'autre (unités de portée, notation de taille, noms de compétences), même quand chaque entrée prise isolément est correcte.
- **Pour les valeurs chiffrées** (PV, dégâts, DC), reconstruisez-les depuis la table officielle plutôt que de vous fier à une relecture visuelle — sur des dizaines d'entrées, l'œil laisse passer des écarts qu'un recalcul systématique attrape immédiatement.

---

*Méthode générale, sans contenu tiré d'un setting particulier. Voir [Fondamentaux Nimble](fondamentaux-nimble.md) pour les règles Nimble elles-mêmes.*
