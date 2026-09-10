# Audit du système de magie Nimble
## Règles extraites des sources primaires (CoreRules, Heroes, GMG)

> Ce document pose les règles exactes telles qu'elles sont écrites dans les PDF Nimble.
> Chaque affirmation est sourcée. Aucune inférence externe.

---

## 1. Résolution des attaques — la règle exacte

> *"Roll the die listed on the spell, weapon, or ability, and deal that much damage. However, if you roll a 1, you miss, and the attack has no effect."*
> *(CoreRules p.13)*

**Ce que ça signifie concrètement :**
- Il n'y a pas de jet d'attaque vs CA/défense active de l'adversaire
- On lance directement les dés de dégâts
- Un 1 sur le dé principal = raté, aucun effet
- Tout autre résultat = touché, les dégâts s'appliquent intégralement

**Le dé principal sur plusieurs dés :**
> *"For attacks with multiple dice, the leftmost die is called the Primary Die. It determines whether the attack is a hit or a miss."*
> *(CoreRules p.13)*

Sur 3d6 : seul le premier dé compte pour rater. Si le premier dé donne 1 = raté. Les autres dés ne peuvent pas faire rater l'attaque. La probabilité de rater reste 1/6 quelle que soit la taille du pool de dés.

**Critique explosif :**
> *"Rolling the max on a Primary Die is a critical hit (crit). When you crit, roll the Primary Die again, and add the result to the total. Repeat this each time you roll the maximum — there's no limit, except your luck! Crits also ignore monster armor."*
> *(CoreRules p.13)*

**Attaques précipitées :**
> *"A hero may attack more than once on their turn, but these additional attacks are rushed, imposing cumulative disadvantage for each additional attack after the first."*
> *(CoreRules p.13)*

---

## 2. L'Armure — deux systèmes distincts

### Armure des héros (active, par réaction)

> *"Armor represents your hero's ability to dodge or block damage when you use the Defend reaction."*
> *(CoreRules p.32)*

> *"Defend: Reduce damage from any single attack by your Armor whenever you use this reaction."*
> *(CoreRules p.14-15)*

**Ce que ça signifie :**
- L'armure ne réduit RIEN passivement
- Elle ne s'applique QUE si le héros utilise sa réaction Défendre
- Défendre coûte 1 action (réaction = 1 action hors de son tour)
- Limité à 1/ronde
- Si le héros ne se Défend pas, il encaisse les dégâts bruts intégralement

**Valeurs d'armure des héros :**

| Type | Armure |
|---|---|
| Aucune / Vêtements | DEX |
| Tissu (Tenue d'aventurier) | 2+DEX |
| Cuir (Peaux bon marché) | 3+DEX |
| Maille rouillée | 6+DEX (max DEX 2) |
| Plaques rouillées | 10 (fixe, sans DEX) |
| Armure complète | 18 (fixe) |
| Mithril | 22 (fixe) |

### Armure des monstres (passive, permanente)

> *"Medium Armor: Just the Dice. Monsters with Medium Armor ignore all damage modifiers from stats and other effects, taking damage from the sum of the dice only."*
> *"Heavy Armor: Half the Dice. Monsters with Heavy Armor ignore damage modifiers and take half the sum of the dice (rounding up)."*
> *(GMG p.24)*

**Ce que ça signifie :**
- Les monstres n'ont pas besoin d'utiliser une réaction — leur armure est passive
- Les critiques ignorent l'armure des monstres
- Certains types de dégâts ignorent certaines armures (tranchant ignore armure lourde, perforant ignore armure moyenne)

**Conséquence pour les sorts :** un sort qui précise "ignore armor" est significativement plus puissant contre des monstres blindés. C'est un marqueur de puissance important à intégrer dans le calibrage.

---

## 3. Points de vie et mort

> *"When reduced to 0 HP, gain 1 Wound; you also gain the Dying condition until you regain HP."*
> *"You die when you have taken 6 Wounds."*
> *(CoreRules p.8)*

**PV de départ par classe (sources primaires) :**

| Classe | PV départ | Dé de vie |
|---|---|---|
| Mage | 10 | 1d6 |
| Tricheur (Cheat) | 10 | 1d6 |
| Tissechant (Songweaver) | 13 | 1d8 |
| Zéphyr | 13 | 1d8 |
| Berger (Shepherd) | 17 | 1d10 |
| Chevalier du Serment (Oathsworn) | 17 | 1d10 |
| Berserker | 20 | 1d12 |

**État Mourant :**
> *"While Dying, actions are limited to 1, Concentration is broken, and you are at risk of further serious harm: Attacking/casting spells causes 1 Wound unless you make a DC 10 STR save. Taking damage while Dying causes 2 Wounds; a crit causes 3 instead."*
> *(CoreRules p.8)*

---

## 4. Le système de magie — structure exacte

### Les six écoles de magie

Nimble dispose de **6 écoles** avec chacune une liste de sorts propre :
- Feu (Fire)
- Glace (Ice)
- Foudre (Lightning)
- Vent (Wind)
- Radieux/Sacré (Radiant)
- Nécrotique (Necrotic)

Chaque école a :
- Des **sorts mineurs (Cantrips)** : gratuits en Mana, 0 coût
- Des **sorts de Rang 1 à 9 (Tiers)** : coût Mana = numéro du rang
- Des **sorts utilitaires (Utility Spells)** : capacités hors combat acquises par aptitude de classe

### Le Mana

**Formule du pool de Mana :**
- Mage : *"(INT×3)+LVL"* *(Heroes p.32)*
- Berger : *"(WIL×3)+LVL"* *(Heroes p.50)*
- Tissechant : *"(INT×3)+LVL"* *(Heroes p.56)*
- Chevalier du Serment : *"WIL + LVL"* *(Heroes p.38)* — pool réduit, cohérent avec son rôle hybride
- Stormshifter : *"(WIL×3)+LVL"* *(Heroes p.61)* — même formule que le Berger, débloqué niv.2
- Shadowmancer : **pas de pool de Mana**. Mécanique à part, *Pilfered Power* — voir note en fin de section.

**Recharge :** lors d'un Repos Sûr (Safe Rest) pour toutes les classes.

**Coût d'un sort :** égal à son rang. Un sort de rang 3 coûte 3 Mana.

**Amplification (Upcasting) :**
> *"Some spells have a greater effect for each additional mana spent on them. A hero can upcast a spell only up to the tier they have unlocked."*
> *(CoreRules p.13)*

**Sorts mineurs :** aucun coût en Mana, toujours disponibles.

### Déblocage des rangs par niveau

Confirmé pour Mage, Berger, Tissechant et **Stormshifter** (progression standard) :

| Rang débloqué | Niveau de classe |
|---|---|
| Sorts mineurs | Niveau 1 |
| Rang 1 | Niveau 2 |
| Rang 2 | Niveau 4 |
| Rang 3 | Niveau 6 |
| Rang 4 | Niveau 8 |
| Rang 5 | Niveau 10 |
| Rang 6 | Niveau 12 |
| Rang 7 | Niveau 14 |
| Rang 8 | Niveau 16 |
| Rang 9 | Niveau 18 |

**Le Chevalier du Serment (Oathsworn) suit une table différente et plafonne au rang 7** *(Heroes p.37-41)* :

| Rang débloqué | Niveau Oathsworn |
|---|---|
| Sorts mineurs | Niveau 1 |
| Rang 1 | Niveau 2 |
| Rang 2 | Niveau 4 |
| Rang 3 | Niveau 6 |
| Rang 4 | Niveau 8 |
| Rang 5 | Niveau 10 |
| Rang 6 | **Niveau 13** |
| Rang 7 | **Niveau 17** |
| Rang 8 / 9 | **Jamais débloqués** |

Le Shadowmancer n'a pas de table de déblocage de rang classique : à partir du niveau où un rang est débloqué (mêmes paliers que la table standard), *tous* ses sorts sont automatiquement lancés à ce rang (pas d'upcast à la carte) — voir *Pilfered Power* ci-dessous.

---

## 5. Qui accède à quelle école

| Classe | Écoles disponibles |
|---|---|
| Mage | Feu + Glace + Foudre (de base). **Correction** : *Elemental Mastery* ne donne PAS de 4e école de combat — seulement les *Utility Spells* des écoles déjà connues. Une 3e école de combat (Nécrotique ou Vent, au choix) vient de la **sous-classe** (Invoker of Control / Invoker of Chaos, niv.7), limitée à 1 cantrip + 1 sort de rang. |
| Berger | Radieux + Nécrotique |
| Tissechant | Vent + 1 école au choix |
| Chevalier du Serment | Radieux uniquement (plafonné au rang 7, voir §4) |
| Stormshifter | Foudre + Vent (de base). Sous-classe *Circle of Sky & Storm* (niv.3) ajoute Glace OU Radieux au choix. |
| Shadowmancer | Nécrotique uniquement (de base, *"Master of Darkness"*). Sous-classe *Pact of the Red Dragon* → +Feu ; *Pact of the Abyssal Depths* → +Glace. Pas de Mana (voir *Pilfered Power* ci-dessous). |

**Conséquence importante :** chaque classe est liée à ses écoles. Un Berger ne peut pas lancer des sorts de Feu. Le catalogue de sorts disponibles est fermé par classe.

**Shadowmancer — Pilfered Power (mécanique sans Mana)** *(Heroes p.61-63)* : au lieu d'un pool de Mana, le Shadowmancer *"vole du pouvoir à son patron"* pour lancer ses sorts au rang le plus élevé débloqué, jusqu'à **DEX fois** avant que son patron ne s'en aperçoive. Chaque dépassement de cette limite inflige au Shadowmancer des dégâts égaux à la moitié de ses PV max. La limite se recharge en communiant avec son patron lors d'un Repos Sûr. Gabarit intéressant pour un Enchanteur ou un pacte fae Dolmenwood à hauts risques.

**Utility Spells — progression complète** *(absente de la version précédente de cet audit)* : l'acquisition ne s'arrête pas au niveau 3.
- Mage (*Elemental Mastery*) : niv.3 (1 école), niv.6 (2e palier), niv.14 (école complète en Utility Spells)
- Berger (*Master of Twilight*) : niv.3 (1 Nécrotique + 1 Radieux), niv.6 (+1 de chaque), niv.11 (toutes les Utility Spells Nécrotique/Radieux)
- Tissechant (*Windbag*) : niv.3 (1/école connue), niv.6 (2e/école), niv.14 (toutes les Utility Spells des écoles connues)

---

## 6. Sorts utilitaires (Utility Spells) — une catégorie distincte

Les **Utility Spells** sont une sous-catégorie de sorts mineurs, hors combat, acquis via des aptitudes de classe spécifiques (pas au niveau 1) :

- Mage : *"Elemental Mastery. Learn the Utility Spells from 1 spell school you know."* — Niveau 3
- Berger : *"Master of Twilight. Choose 1 Necrotic and 1 Radiant Utility Spell."* — Niveau 3
- Tissechant : *"Windbag. Choose 1 Utility Spell from each spell school you know."* — Niveau 3

**Ce que ça signifie pour notre conversion :** les sorts hors combat de Dolmenwood (Detect Evil, Purify Food, Speak with Animals…) correspondent exactement à cette catégorie. Ils s'intègrent naturellement comme Utility Spells, sans toucher aux sorts de combat.

---

## 7. Calibrage — ce que les règles permettent de déduire

### Sorts mineurs offensifs — échantillon sourcé

| Sort | École | Dés | Effet secondaire |
|---|---|---|---|
| Flame Dart | Feu | 1d10 | Smoldering sur critique |
| Ice Lance | Glace | 1d6 | Slowed sur touche |
| Snowblind | Glace | 1d6 Reach 1 | Blinded 1 tour |
| Razor Wind | Vent | 1d4 Vicious | Blesse 1 cible adjacente |
| Rebuke | Radieux | 1d6 ignore armure | ×2 contre morts-vivants *ou cibles "lâches" (Frightened/à couvert)* |
| Entice *(anciennement traduit « Attraction »)* | Nécrotique | 1d4 ignore armure | Rapproche de 2 cases |

**Observation :** les sorts mineurs offensifs varient de 1d4 à 1d10 selon la portée et l'effet. Un sort à portée courte (Reach 1) ou avec un effet limité peut aller jusqu'à 1d6. Un sort à longue portée (Range 8-12) sans effet secondaire peut monter à 1d10. La relation portée/puissance est inversée : plus la portée est grande, plus le dé de dégâts est petit.

**Exception notable :** Rebuke (1d6 ignore armure, ne rate jamais) est calibré conservativement malgré ses propriétés — le "ne rate jamais" compense le dé plus petit.

### Sorts de rang 1 — échantillon sourcé

| Sort | École | Actions | Dés | Notes |
|---|---|---|---|---|
| Heal | Radieux | 1 | 1d6+KEY | Soin, pas dégâts |
| Lifebinding Spirit | Radieux | 1 | Invocation | Berger uniquement |
| Blustery Gale | Vent | 2 | 3d4 | + déplacement forcé |
| Arc Lightning | Foudre | 2 | 3d8 | Chaîne à cible suivante |
| Frost Shield | Glace | 1 | — | Réaction : 2×KEY PVTemp + Défendre gratuit |
| Shadow Trap | Nécrotique | 2 | 3d12 | Concentration, piège au sol |

**Observation clé :** les sorts de rang 1 offensifs coûtent systématiquement **2 actions** et font environ 3 dés (3d4 à 3d12 selon l'école). Les sorts de soutien/réaction coûtent 1 action. C'est la règle structurante du rang 1.

### Sorts de rang 2 — observation

Les sorts de rang 2 sont souvent des **effets durables ou défensifs** (concentration, réactions) plutôt que des dégâts supérieurs au rang 1. Shatter (3d6, 2 actions) est l'exception offensive, avec une condition sur les cibles Hampered.

---

## 8. Ce que ce calibrage interdit pour nos sorts Dolmenwood

Sur la base des règles exactes, un sort Dolmenwood converti ne devra jamais :

1. **Faire plus de dégâts qu'un sort Nimble de même rang** à nombre d'actions égal
2. **Combiner dégâts + ignore armure + effet secondaire** en 1 action au rang 1 (Rebuke le fait, mais ses dégâts sont faibles en conséquence)
3. **Fonctionner en 1 action pour des dégâts de zone** avant le rang 3 minimum
4. **Ignorer le dé principal** pour la détermination du raté — tous nos sorts multi-dés auront un dé principal à gauche
5. **Dépasser le pool de Mana disponible** — à niveau 2, un Berger avec WIL +2 a (2×3)+2 = 8 Mana. Un sort de rang 4 consomme la moitié de son pool journalier. C'est la borne à ne pas franchir pour les effets "normaux"

---

---

## 9. Fondamentaux transversaux Nimble — à respecter pour TOUT contenu homebrew (Kindreds, Glamours, Runes, sorts)

*Ajouté suite à un audit ciblé sur l'esprit des règles et la cohérence des probabilités — nécessaire avant de calibrer quoi que ce soit de nouveau.*

### Avantage / Désavantage — mécanique de pool de dés, pas "2d20 garder le meilleur"

> *"If you are ever in a favorable situation, the GM may allow you to roll with advantage. To do this, roll 1 additional die of the same type and remove the lowest... If you have multiple instances of advantage or disadvantage, for each one, roll an extra die... Each instance of advantage cancels out one instance of disadvantage before your roll."* *(CoreRules p.9)*

S'applique uniformément aux tests de compétence, JdS, attaques ET dégâts (ex. "Greataxe 2d6 avec avantage" = ajouter 1d6, retirer le plus bas). Pour un test d20 simple, le résultat net est identique à la 5e (ajouter 1d20, garder le meilleur), mais le principe est généralisable à n'importe quel pool de dés — utile si on veut donner de l'avantage sur un jet de dégâts d'un sort Dolmenwood plutôt que sur son jet de résolution.

**Chaque héros a des sauvegardes nativement avantagées/désavantagées selon sa classe** (Prime Abilities +/–), même mécanique de dé.

### Seuils de Difficulté (DC) — deux régimes bien distincts

**a) Test de compétence d'un héros** *(CoreRules p.8)* — table fixe, non liée au niveau, plafond de compétence +12 :

| Difficulté | DC | Exemple |
|---|---|---|
| Facile | 8 | Repérer un ogre accroupi derrière un buisson |
| Moyen | 12 | Trouver une porte cachée derrière une bibliothèque |
| Difficile | 15 | Calmer un Hibou-Ours blessé pris au piège |
| Très difficile | 18 | Percer les véritables intentions d'un espion entraîné |
| Extrêmement difficile | 20+ | Désamorcer un piège légendaire ancien |

**b) DC d'un effet imposé par un HÉROS** (sort, capacité de classe, capacité d'Ascendance) : **10+KEY**, la stat clé pertinente *(CoreRules p.9 et p.45)*. C'est la formule à utiliser pour tout Glamour, Rune, ou trait de Kindred qui impose un JdS — **jamais** la table de monstre ci-dessous.

**c) DC d'un effet imposé par un MONSTRE/PNJ** : table liée au **niveau du monstre**, pas de formule 10+stat *(GMG p.29, Monster Builder)* :

| Niveau monstre | 1/4 | 1/2 | 1 | 4 | 6 | 8 | 10 | 14 | 18 | 20 |
|---|---|---|---|---|---|---|---|---|---|---|
| Save DC | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 17 | 19 | 19 |

*(Table Legendary Monster Builder, GMG p.43, similaire : Niv1→10, Niv5→12, Niv10→15, Niv15→17, Niv20→20.)*

### Ascendances natives Nimble — le budget de puissance de référence

*(CoreRules p.23-27, "Common/Exotic Ancestries")* — patron constant à respecter pour toute Ascendance Dolmenwood :

- **+1 fixe permanent maximum** sur une seule stat/compétence/vitesse/armure (jamais +2 en permanent inconditionnel).
- Toute capacité plus forte que +1 est rendue **à charges** : 1×/Repos Sûr ou 1×/rencontre, jamais passive illimitée.
- Exemples exacts : Human *"Tenacious. +1 to all skills and Initiative."* — Halfling *"Elusive. +1 to Stealth. If you fail a save, you can succeed instead, 1/Safe Rest."* — Orc *"Relentless. When you would drop to 0 HP, you may set your HP to LVL instead, 1/Safe Rest."* — Kobold (exotique, budget plus large) *"+3 to Influence friendly characters."*
- Confirmation indirecte : les "Minor Boons" achetables (objets, GMG p.21) utilisent le même calibre (+1 initiative, +1 mana, +1 dégâts feu, +1 vitesse) — le +1 est la norme du "petit bonus" dans tout Nimble, gratuit ou payant.

**Conséquence pour nos Kindreds Dolmenwood** : un bonus de +2 fixe et permanent (comme la Beauté d'outre-monde ou la Résistance à la magie de l'Elfe/Grimalkin, fidèles à la source OSE) dépasse ce budget. Ce n'est pas forcément à corriger — Dolmenwood a ses propres Kindreds emblématiques et plus "chargés" que les Ascendances Nimble de base — mais c'est un écart **conscient** à trancher au cas par cas, pas un oubli.

### Dégâts fixes qui scalent avec le niveau — anti-pattern explicitement déconseillé

> *"Magical items that only provide a flat stat or damage boost are fun–in the fleeting moment a hero receives them. But these bonuses are quickly forgotten–rolled into the base math of the game. It just inflates the numbers and forces you to rebalance encounters around it."* *(GMG p.18)*

**Aucune arme Nimble ne voit son dé de dégâts grossir avec le niveau** — la progression vient de la stat clé (qui augmente lentement) et des dés de ressource de classe (qui grossissent, eux : Berserker d4→d12, Cheat 1d6→3d20). **Ne pas transposer telles quelles les tables de progression OSE qui font grossir un dégât fixe avec le niveau** (ex. la table de Cornes du Breggle 1d4→1d6+2) — elles deviennent négligeables dès le niveau 8-10 dans la courbe Nimble. Convertir plutôt en arme naturelle à dé fixe (+ FOR), avec éventuellement une propriété (Vicieuse, Reach) débloquée à un palier de Kindred, jamais un scaling numérique linéaire.

### Bonus : table de conversion 5e → Nimble (GMG p.109-110, section "5e Conversion")

Utile pour tout le reste du travail de conversion (pas seulement la magie) :
- **JdS** : CON save → JdS FOR ; WIS/CHA save → JdS VOL.
- **Compétences** : Animal Handling/Nature/Survival → Naturecraft ; Athletics → Might ; Deception/Persuasion/Performance → Influence ; History/Religion → Lore ; Investigation/Medicine → Examination ; Sleight of Hand/Acrobatics → Finesse.
- **Conditions** : Paralyzed/Stunned/Unconscious → Incapacitated.
- **Monstres** : CA 5e 14-17 → Armure Moyenne ; moins → sans armure ; plus → Armure Lourde. Garder les dés de dégâts 5e tels quels.
- **Tests de compétence de monstre sans stat Nimble** : aucun bonus ou +1d4 (non entraîné) ; +1d6 à +1d10 (entraîné/très bon) ; +1d12 à +1d20 (classe mondiale/légendaire).

---

*Document établi depuis les sources primaires CoreRulesv1.0, Heroesv1.0 et GMGv1.0 Nimble. Aucune inférence externe.*