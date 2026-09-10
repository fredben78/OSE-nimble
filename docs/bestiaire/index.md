# Dolmenwood sous Nimble — Conversion du Bestiaire

> Statut : **méthodologie validée, et les 158 créatures converties** dans le dossier `bestiaire/` (un .md complet par créature — 87 Bestiary + 53 Animaux + 18 PNJ génériques). Ce document garde son rôle de référence méthodologique ; les 3 conversions témoins ci-dessous restent illustratives mais **le dossier `bestiaire/` fait foi** en cas d'écart. Une relecture croisée a normalisé la terminologie (portée toujours notée `Reach N`, taille toujours `Petit`/`Grand`/omise si Moyen) sur les 158 fichiers, mais de petits écarts de calibrage subsistent d'un lot à l'autre (choix du dé de dégâts, application du cran de rétrogradation) — ce sont des jugements de design indépendants, pas des erreurs de règle. Par exemple, le Sanglier et le Barrowbogey ci-dessous diffèrent légèrement de leurs versions finales dans `bestiaire/boar.md` et `bestiaire/barrowbogey.md` (dé d8 vs d10, cran de rétrogradation appliqué ou non) : les deux sont défendables, seule la version du dossier est à utiliser en jeu.

---

## 1. Pourquoi cette conversion est plus simple qu'elle n'y paraît

Deux coïncidences structurelles entre Dolmenwood (OSE) et Nimble rendent la conversion mécanique plutôt qu'inventive :

1. **Le champ "Level" existe déjà côté Dolmenwood** et joue le même rôle que le "Level" du Monster Builder Nimble : un monstre de niveau N est calibré comme un défi pour un groupe de niveau N, dans les deux systèmes. **On réutilise directement le Level Dolmenwood comme clé d'entrée dans la table Nimble** — pas de formule de conversion HD→Niveau à inventer. Les niveaux fractionnaires (1/4, 1/3, 1/2) existent aussi des deux côtés pour les créatures faibles.
2. **La CA Dolmenwood est déjà ascendante et dans la même plage numérique que la 5e** (Boar CA12, Barrowbogey CA13, Wyrm—Blood CA19). La seule table de conversion d'armure du GMG Nimble (prévue pour la 5e) s'applique donc telle quelle.

## 2. Méthode de conversion, étape par étape

1. **Niveau** : reprendre le Level Dolmenwood tel quel.
2. **PV, Dégâts/round, Save DC** : lire la ligne correspondante dans la table Monster Builder Nimble (GMG p.29).
3. **Armure** : depuis la CA Dolmenwood — **CA 14-17 → Armure Moyenne, moins → Sans armure, plus → Armure Lourde** (règle GMG p.109-110, transposée directement).
4. **Taille de dé de dégâts**, choisie selon le Type Dolmenwood (thème visuel, pas de règle stricte) :
   - Undead → d4 (lent, gros bonus fixe) · Fairy/petit humanoïde chaotique → d6 · Mortal/humanoïde standard → d8 (défaut) · Animal/Bête → d10 · Géant/Construct massif → d12 · Dragon majeur/entité cosmique → d20.
5. **Capacités spéciales** : traduire chaque capacité en prose Dolmenwood vers le format Nimble (déclencheur en italique + effet court), en piochant dans le catalogue *Flavorful Monster Abilities* (GMG p.30) quand un équivalent existe, sinon en écrivant une entrée sur mesure dans le même style. **Règle de coût** (GMG p.29) : chaque capacité ajoutée fait baisser PV ou dégâts d'1 cran dans la table, ou traite le monstre comme 1 niveau plus fort — à appliquer surtout aux créatures qui cumulent 3+ capacités (les Wyrms, par ex.).
6. **Boss solo unique** (un seul exemplaire rencontré, avec du lore propre — typiquement les Wyrms nommés, certaines Drunes, PNJ majeurs) → utiliser le **Legendary Monster Builder** (GMG p.41-44) à la place, calé sur le niveau du **groupe de joueurs** plutôt que sur un niveau de monstre isolé.
7. **Moral** : Nimble n'a pas de système de moral formel — le Moral Dolmenwood (ex. Morale 9) devient une **indication narrative pour le MJ** ("cette créature est du genre à se battre jusqu'au bout" vs "fuira si la situation tourne mal"), pas un jet automatique.

---

## 3. Conversions témoins

### 3a. Boar *(Sanglier — Appendice, cas simple)*

**Description** *(VO : « Omnivorous wild boars that dwell throughout Dolmenwood. Irascible and dangerous, if disturbed. »)* :
> Sangliers omnivores qui vivent à travers tout le Dolmenwood. Irascibles et dangereux si on les dérange.

**Source** : Level 3, AC 12, HD 3d8 (13 PV), Att Tusk (+2, 2d4), Speed 50, Morale 9. Aucune capacité spéciale.

**Conversion Nimble** (niveau 3 : 41 PV sans armure / dégâts 15/round, table p.29 ; CA12 < 14 → sans armure ; Type Animal → dé d10) :

> **SANGLIER** LVL 3 — ♥41
> **Défenses de coin.** 2d8+6 (Reach 1). Sur un critique : la cible est Prone (renversée par la charge).

*Pas de capacité spéciale ajoutée dans la source → on reste sur les PV/dégâts de base de la table, pas de malus à appliquer.*

### 3b. Barrowbogey *(fae moyenne, cas intermédiaire)*

**Description** *(VO : « Waif-like fairies (3′ tall) with saggy, wrinkled skin. Carry pots or jugs on their shoulders in place of heads. Lair in barrow mounds, riddled with tunnels extending into fairy roads. »)* :
> Fées chétives (90 cm) à la peau flasque et ridée. Portent des pots ou des cruches sur les épaules en guise de tête. Nichent dans des tumulus percés de tunnels qui rejoignent les routes féeriques.

**Comportement** *(VO : « Sharp-witted, wild, tricksome »)* : vif d'esprit, sauvage, farceur.
**Discours** *(VO : « Tinny voix emanating from head-pot. Sylvan, Woldish (1-in-3 chance) »)* : voix métallique et creuse sortant du pot-tête. Parle le Sylvan, et le Woldish avec 1 chance sur 3.
**Possessions** : aucune. **Trésor** : catégorie C4 + R4 + M1, plus 4d20 pots ou cruches.

**Source** : Level 3, AC 13, HD 3d8 (13 PV), Attaques (2 griffes +2/1d4, ou 2 fléchettes de ronces +2/1d4 à distance), Speed 40, Morale 9. Capacités : vulnérabilité au fer froid, vision dans le noir, malédiction de la demeure (1×/jour, perte de FOR/DEX/CHA), destruction du pot à la mort.

**Conversion Nimble** (niveau 3 : 41 PV sans armure / 15 dégâts/round, table p.29 ; CA13 < 14 → sans armure ; Type Fairy/petit chaotique → d6 ; 2 capacités ajoutées → on descend d'1 cran dans la table, soit les valeurs du niveau 2 : 34 PV / 13 dégâts) :

> **BARROWBOGEY** LVL 3, SMALL — ♥34
> *Vulnérable au fer froid. Les armes en fer froid infligent +1 dégât fixe.*
> *Fuite en éclats. À la mort, le pot-tête de la créature se brise instantanément — aucun butin sur le corps.*
> **Griffes** ou **Fléchette de ronces.** 2d6+4 (Reach 1, ou Range 8 pour les fléchettes).
> **Malédiction de la demeure** *(1×/jour, hors combat, action)* : cible une habitation. Tous ceux qui y séjournent doivent réussir un JdS FOR (SD 10+VOL) ou subir -1 FOR/-1 DEX/-1 Influence (tremblements, furoncles) jusqu'à dissipation (*Remove Curse*/*Hex Weaving*, ou manger une bouillie cuite dans le pot volé au fae responsable).

*Vision dans le noir omise du stat-bloc (par défaut chez la plupart des fae, à noter au niveau du Type plutôt que répété à chaque créature).*

**Notes de lore additionnelles** *(non mécaniques, à garder pour le rôle-play)* :
- **Pots et tourtes** : les Barrowbogeys adorent les tourtes et les récipients en terre cuite (ils n'en fabriquent pas eux-mêmes). On peut les amadouer avec de tels cadeaux ; ils s'introduisent parfois dans les villages pour en voler aux mortels.
- **Relation avec les morts-vivants** : les Barrowbogeys cohabitent parfois avec des morts-vivants — les deux parties s'ignorent généralement.
- *(Le livre source fournit aussi des tables de Traits (1d6), Rencontres (1d4), Repaires (1d4) et une liste de noms — Fiddlethumb, Hob, Jack-a-Napes, Nob, Tom-a-Merry, Willbegone — à reprendre telles quelles pour le MJ, non dupliquées ici.)*

### 3c. Wyrm—Blood *(dragon signature, cas complexe → Legendary)*

**Description** *(VO : « 50′ long, with deep crimson scales, human-like faces, pupilless blue eyes, a ridge of antlers at the neck, and a thorny, whip-like tail. Often charm lesser beings to do their bidding. »)* :
> Long de 15 mètres, écailles pourpre profond, visage quasi-humain, yeux bleus sans pupille, une crête de bois de cerf à la nuque, et une queue épineuse en forme de fouet. Charme souvent des créatures inférieures pour qu'elles fassent sa volonté.

**Comportement** *(VO : « Scheming, cruel, sadistic »)* : calculateur, cruel, sadique.
**Discours** *(VO : « Eloquent, venomous. Woldish, Wyrm, Sylvan »)* : éloquent, venimeux. Parle le Woldish, le Wyrm (langue propre aux dragons) et le Sylvan.
**Possessions** : aucune. **Trésor** : catégorie C10 + R8 + M11 (un trésor de dragon conséquent).
**Repaire** : 50% de chances d'être endormi si rencontré dans son antre.

**Source** : Level 9, AC 19, HD 9d8 (40 PV), Attaques (morsure +7/2d10 + queue +7/2d6, ou souffle de sang bouillant), Speed 80/Vol 80, Morale 9. Capacités : immunités multiples (magie/armes magiques seulement, immunisé acide/poison, immunisé feu-foudre-froid mondain, mi-dégâts si magique), souffle 3×/jour (dégâts = PV actuels, zone), voix charmeuse (JdS Sort, domination totale), vol magique, vulnérabilité unique par individu, régénération (renvoi Wyrm—Overview).

**C'est un cas Legendary** : créature unique, nommée, avec du lore propre et plusieurs mécaniques qui redéfinissent le combat (charme de masse, souffle proportionnel aux PV restants, vulnérabilité secrète). On calibre sur le **niveau du groupe de héros** plutôt que sur son propre niveau isolé — pour un groupe de niveau 9 (table Legendary p.43 : PV Armure Lourde 195, Last Stand 90, DC 14, petite action 16 dégâts, grande action 32 dégâts ; CA19 → Armure Lourde confirmée) :

> **WYRM DE SANG** *(Boss Légendaire, groupe de Niveau 9)* — ♥195 (Armure Lourde), STR+ INT–
> *Immunités. Seuls les armes/effets magiques le blessent. Immunisé à l'acide et au poison. Immunisé au feu/foudre/froid non-magiques ; mi-dégâts si magiques.*
> *Voix charmeuse. En fin de tour, cible 1 héros en vue : JdS VOL (SD 10+VOL du Wyrm ≈ 14) ou Charmé — avance vers le Wyrm, lui obéit, le défend, ne peut plus attaquer ni lancer de sort tant qu'il est charmé. Se rompt si le Wyrm est tué ou subit des dégâts d'un allié du charmé.*
> **ACTIONS** *(après le tour de chaque héros, choisir)* :
> — **Morsure et Queue** *(petite action, mobilité)* : déplacement 8 cases (vol) + morsure 3d8+4 (16 dégâts moy.) OU coup de queue qui repousse 2 cases.
> — **Souffle de Sang Bouillant** *(grande action, 3×/rencontre max)* : ligne de 3×20 cases, dégâts = ses PV actuels (JdS DEX pour moitié, SD 14).
> **BLOODIED** *(à 97 PV)* : le Wyrm gagne une 3e option d'action : **Domination Totale** — tente de charmer jusqu'à 2 cibles au lieu d'1 en fin de tour.
> **LAST STAND** *(à 0 PV, 90 dégâts avant destruction réelle)* : le Wyrm, agonisant, n'utilise plus que Souffle de Sang Bouillant chaque activation, sans limite de fréquence.
> *Vulnérabilité secrète (choisie par le MJ, ex. lumière du jour, terre consacrée, corne de licorne) : les dégâts subis de cette source ignorent toutes les immunités et infligent un critique automatique.*

*Régénération naturelle et vulnérabilité unique par individu : voir Wyrm—Overview (p.96 du Monster Book), qui renvoie à un traitement transversal aux 4 variantes (Bile Noire/Phlegme/Sang/Bile Jaune, associées aux 4 humeurs médiévales). Le patron ci-dessus se réutilise pour les 3 autres Wyrms en changeant le type de souffle et d'immunité.*

---

## 4. Bestiaire complet — statut final

Le découpage en 11 lots (par plage de pages, traités en parallèle par des agents en arrière-plan) est terminé : **158 fichiers dans `bestiaire/`**, un par créature — 87 Bestiary signature (dont les 4 Wyrms et les 13 Drune—Audrune en traitement Legendary), 53 Animaux d'Appendice, 18 PNJ génériques (9 Adventurers × 3 niveaux, 9 Everyday Mortals).

**Relecture croisée effectuée** : normalisation de la terminologie (portée toujours `Reach N`, taille toujours `Petit`/`Grand`/omise par défaut si Moyen) sur l'ensemble des 158 fichiers, plus vérification de complétude (aucun trou, aucun doublon) après plusieurs coupures de session en cours de traitement. Les petits écarts de calibrage entre lots (choix de dé, application du cran de rétrogradation) sont documentés comme variance de jugement acceptable, pas comme erreurs — voir la note en tête de document.

**Ce qui pourrait encore être affiné** (non bloquant pour jouer) :
- Vérifier au cas par cas que le cran de rétrogradation (2+ capacités → -1 niveau) a été appliqué avec la même sévérité d'un lot à l'autre.
- Harmoniser le style de description entre lots (certains sont plus littéraires, d'autres plus secs).
- Décider si les Drune—Audrune (13 fiches Legendary individuelles) doivent être condensées en un seul gabarit + variantes plutôt que 13 blocs complets.

---

*Document de travail. Méthodologie basée sur GMGv1.0 Nimble (Monster Builder p.29, Legendary Monster Builder p.41-44, conversion d'armure p.109-110) et Dolmenwood Monster Book 2024-08-06.*
