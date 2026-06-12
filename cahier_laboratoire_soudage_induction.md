# Cahier de laboratoire — Campagne de soudage par induction semi-statique

**Projet** : Mitigation du fiber flow / squeeze-out en soudage par induction semi-statique de laminés CF-PEKK
**Configuration** : Pression de consolidation transmise par le concentrateur de flux via céramique d'espacement
**Auteur** : Maxence Dubois
**Institution** : ÉTS — Montréal
**Période de la campagne** : 11 / 06 / 2026 → ____ / ____ / 2026
**Version du document** : 0.1 

---

## 0. Conventions du document

- Les balises `[INSÉRER ...]` marquent les emplacements de données visuelles ou graphiques à intégrer.
- Les champs `______` sont à remplir manuellement après chaque essai.
- Identifiant d'essai : `<Série>-<n°>` (ex. A-1, B-2, C-3).
- Toute déviation au protocole est consignée dans la section « Déviations et observations » de la fiche d'essai concernée, jamais corrigée silencieusement.
- Unités : SI sauf mention contraire (pression en MPa ou kPa, courant en A, temps en s, dimensions en mm).

---

# PARTIE 1 — SÉRIE A : BASELINE (travail effectué)

## 1.1 Objectif de la série

Caractériser le défaut de fiber flow / squeeze-out dans la configuration de référence (sans confinement latéral, pression de référence), afin d'établir une baseline quantifiée pour les séries de mitigation B et C.

## 1.2 Description du montage expérimental

### 1.2.1 Empilement et matériaux

| Élément | Spécification                                                                                                                                      |
|---|----------------------------------------------------------------------------------------------------------------------------------------------------|
| Laminé supérieur | CF-PEKK, empilement [45/-45/0/90]₃ₛ + **pli twill en surface supérieure** (couche suscepteur, maximisation de la chauffe par courants de Foucault) |
| Laminé inférieur | CF-PEKK, empilement [45/-45/0/90]₃ₛ                                                                                                                |
| Interface de soudage | Film PEKK néat, épaisseur 0,004 po (~0,10 mm)                                                                                                      |
| Dimensions laminés | 120 × 40 × 3,36 mm (à consigner)                                                                                                                   |
| Recouvrement (overlap) | 120 x 40 mm                                                                                                                                        |
| Lot matière / traçabilité | ????                                                                                                                                               |

### 1.2.2 Chaîne de transmission de la pression

```
Vérin hydraulique
   ↓
Concentrateur de flux (+ bobine d'induction)
   ↓
Céramique d'espacement (épaisseur : 2 mm, matériau : ??????)
   ↓
Laminé supérieur [twill en surface]
   ↓
Film PEKK 0,004 po (interface de soudage)
   ↓
Laminé inférieur
   ↓
Céramique (matériau : ?????)
```

**Caractéristique distinctive du setup** : la pression de consolidation est appliquée via un vérin hydraulique qui applique la pression directement sur le concentrateur de flux. Cette pression qui passe par la concentrateur de flux est ensuite transmise à la céramique d'espacement afin d'assurer une pression uniforme sur le laminé équipé d'un twill. 

**Aucun confinement latéral** des bords du laminé dans cette série.

`[INSÉRER PHOTO DU MONTAGE DE SOUDAGE — vue d'ensemble]`
`[INSÉRER PHOTO DU MONTAGE DE SOUDAGE — gros plan concentrateur / céramique / laminé]`
`[INSÉRER SCHÉMA COTÉ DU MONTAGE]`

### 1.2.3 Paramètres du générateur d'induction

| Paramètre                                     | Valeur                                                |
|-----------------------------------------------|-------------------------------------------------------|
| Générateur (marque / modèle)                  | Ambrell ???                                           |
| Fréquence                                     | ??? kHz (imposée par le générateur)                   |
| Distance bobine–laminé (distance de couplage) | 2 mm (assurée par céramique d'espacement)             |
| Instrumentation température                   | 5 thermocouples de type K (dans le futur des types E) |
| Acquisition                                   | Cellule d'acquisition National Instruments (LabView)  |

## 1.3 Fiches d'essai — Série A

### Fiche A-1

| Champ | Valeur                     |
|---|----------------------------|
| Date | 05/06/2026                 |
| Courant de consigne | **250 A**                  |
| Durée de chauffe | 1400 sec.                  |
| Pression appliquée | 70 N (valeur de référence) |
| Phase d'application de la pression | Chauffe + Refroidissement  |
| Température max atteinte (interface) | 398 °C                     |
| Refroidissement | Naturel (sous pression)

`[INSÉRER COURBE DE CYCLE DE SOUDAGE — température et courant vs temps, essai A-1]`
`[INSÉRER PHOTOS MACRO AVANT/APRÈS DE L'ÉCHANTILLON A-1]`

**Observations qualitatives** :
Traces de ma céramique qui a collé à la paroie du laminé (Twill).Squeeze-out latéral de matrice observé sur les bords du joint : la matrice fondue du laminé supérieur, sous l'effet combiné de la chute de viscosité (chauffe maximale dans le twill) et de la pression non confinée, est expulsée latéralement. Le fluage de la matrice entraîne un déplacement de fibres (fiber flow) et une distorsion des plis du tissu twill (écrasement local, perte d'épaisseur).

- Étendue du squeeze-out (côté 1 / côté 2) : ______ / ______ mm
- Localisation : Les squeeze-out sont situés aux mêmes emplacements où j'ai posé mon concentrateur de flux lors des cycles de chauffe. 
- Autres observations : Chaque thermocouples passe au dessus de la température de melting. Et même certains passe deux fois la température de transition vitreuse. 

**Déviations et observations** : Les résultats des thermocouples sont assez cohérents comparé aux résultats des thermocouples obtenus avec la chauffe à @200A. Aucun signe de thermocouple qui dysfonctionne.

Cependant j'ai attendu beaucoup trop longtemps entre chaque passe du coil pour changer de spot j'aurais du arrêter la pression en dessous de 120°C puis passer au prochain spot de soudage. 

---

### Fiche A-2

| Champ | Valeur     |
|---|------------|
| Date | 09/06/2026 |
| Courant de consigne | **250 A**  |
| Durée de chauffe | 1250 sec.  |
| Pression appliquée | 50 N ?     |
| Température max atteinte (interface) | 424°C °C   |

`[INSÉRER COURBE DE CYCLE DE SOUDAGE — essai A-2]`
`[INSÉRER PHOTOS MACRO AVANT/APRÈS DE L'ÉCHANTILLON A-2]`

**Observations qualitatives** : Reproduction du défaut observé en A-1 (squeeze-out + distorsion du twill). Juste une trace de ma céramique qui a collée à la paroie du laminé (Twill).

**Comparaison A-1 vs A-2 (répétabilité à 250 A)** : Point positif : On observe le même schéma de chauffe de thermocouple (mise à part TC3). 

**Déviations et observations** : L'un de mes thermocouples à décider de ne pas fonctionner correctement. Correction : Changer le fil de ce thermocouple. 

---

### Fiche A-3

| Champ | Valeur     |
|---|------------|
| Date | 05/06/2026 |
| Courant de consigne | **200 A**  |
| Durée de chauffe | 3300 s     |
| Pression appliquée | 70 N       |
| Température max atteinte (interface) | 400 °C     |

![Échantillon A-3 (Courbes)](/Users/maxencedubois/PycharmProjects/Memoire_Soudage_InductionV2/images/courbe_200A_serieA.png)
`[INSÉRER PHOTOS MACRO AVANT/APRÈS DE L'ÉCHANTILLON A-3]`

**Observations qualitatives** : Défauts de fiber flow présents également à courant réduit. Mais aucun signe d'effets de bords. Juste une trace de ma céramique qui a collée à la paroie du laminé (Twill).

**Déviations et observations** : Chaque thermocouples passe au moins une fois par Tprocessing. Et certains thermocouples passe deux fois au dessus de Tg. 

---

## 1.4 Synthèse Série A

**Constat central** : le fiber flow / squeeze-out est **systématique** (3/3 essais) dans la configuration sans confinement, aux deux niveaux de courant testés. Le défaut se concentre dans le laminé supérieur, au droit de la zone de chauffe maximale (twill), là où la pression est appliquée.

**Mécanisme proposé (hypothèse de travail)** :
1. Le twill supérieur concentre les courants de Foucault → chauffe maximale en surface supérieure.
2. La matrice PEKK du laminé supérieur atteint une viscosité très faible localement.
3. La pression transmise par la céramique, sans confinement latéral, expulse la matrice fondue vers les bords libres.
4. Les fibres du twill, non maintenues, sont entraînées avec la matrice → fiber flow + distorsion de plis.

`[INSÉRER MICROGRAPHIES DES COUPES — A-1, A-2, A-3, plan de coupe et grossissement standardisés]`
`[INSÉRER SCHÉMA DU MÉCANISME EN 3 ÉTAPES — avant / pendant / après]`

**Métriques baseline mesurées** (voir grille §3 ; à remplir) :

| Métrique | A-1 | A-2 | A-3 |
|---|---|---|---|
| Largeur du bourrelet de squeeze-out (mm) | ______ | ______ | ______ |
| Épaisseur résiduelle du pli twill (µm) | ______ | ______ | ______ |
| Perte d'épaisseur locale du joint (%) | ______ | ______ | ______ |
| Angle de waviness max (°) | ______ | ______ | ______ |

---

# PARTIE 2 — SÉRIES B ET C : PROTOCOLE OPÉRATOIRE (à exécuter)

## Logique d'isolement des variables

| Série | Pression | Confinement latéral | Variable isolée |
|---|---|---|---|
| A (baseline) | Référence | Non | — |
| B | **Réduite, constante (chauffe + refroidissement)** | Non | Effet de la pression seule |
| C | Identique à B | **Oui (parois céramique)** | Effet du confinement seul |

⚠️ **Règle d'or** : ne jamais changer deux variables entre deux séries comparées. B ne diffère de A que par la pression ; C ne diffère de B que par le confinement. Tous les autres paramètres (courant, durée, gap bobine, empilement, film) restent **strictement identiques** entre B et C, et identiques à A sauf mention explicite.

---

## 2.1 SÉRIE B — Isolement de l'effet pression (n = 3)

### 2.1.1 Objectif

Déterminer si une pression réduite, appliquée de façon constante pendant toute la chauffe **et** maintenue pendant le refroidissement, suffit à réduire le squeeze-out sans confinement latéral — et quantifier l'effet résiduel.

### 2.1.2 Paramètres fixés

| Paramètre | Valeur | Justification |
|---|---|---|
| Courant | ______ A (choisir UNE valeur de la série A, recommandé : 250 A, cas le plus sévère) | Comparabilité directe avec baseline |
| Pression | ______ (réduite, à fixer avant B-1 et ne plus changer) | Variable d'étude |
| Profil de pression | Constante, appliquée avant le début de chauffe, maintenue jusqu'à T < ______ °C (sous Tg du PEKK, ~160 °C) | Consolidation pendant solidification |
| Durée de chauffe | Identique Série A : ______ s | Comparabilité |
| Empilement / film / gap | Identiques Série A | Comparabilité |
| Confinement latéral | **Aucun** | Isolement de la variable pression |

### 2.1.3 Procédure étape par étape (par essai)

1. **Préparation** : découper et ébavurer les laminés ; mesurer et consigner dimensions et masse de chaque laminé (`______ mm`, `______ g`). Photographier chaque laminé individuellement (voir standard photo §2.2.5).
2. **Empilement** : positionner laminé inférieur / film PEKK 0,004 po / laminé supérieur (twill vers le haut). Vérifier l'alignement du recouvrement à ± 0,5 mm.
3. **Mise en place** : positionner la céramique d'espacement, descendre le concentrateur. Vérifier le gap bobine–laminé : ______ mm (identique Série A).
4. **Pré-charge** : appliquer la pression réduite cible ______ et la stabiliser. Consigner la lecture du manomètre / capteur : ______.
5. **Instrumentation** : vérifier les thermocouples (positions identiques à la Série A), lancer l'acquisition.
6. **Chauffe** : lancer le cycle à ______ A pendant ______ s. Ne pas toucher à la pression pendant la chauffe.
7. **Refroidissement sous pression** : maintenir la pression constante jusqu'à T_interface < ______ °C. Consigner la durée totale sous pression : ______ s.
8. **Démontage** : relever la pression, remonter le concentrateur, extraire l'échantillon. Photographier immédiatement (standard §2.2.5).
9. **Mesures post-essai** : grille de métriques §3 dans les 24 h.

### 2.1.4 Fiches d'essai B-1, B-2, B-3

(Dupliquer la structure de fiche ci-dessous pour chaque essai.)

| Champ | Valeur |
|---|---|
| ID essai / Date | B-__ / ______ |
| Courant / durée | ______ A / ______ s |
| Pression mesurée (pas seulement consigne) | ______ |
| Durée totale sous pression | ______ s |
| T max interface / surface | ______ / ______ °C |
| T à la levée de pression | ______ °C |

`[INSÉRER COURBE DE CYCLE DE SOUDAGE — température, courant ET pression vs temps]`
`[INSÉRER PHOTOS MACRO AVANT/APRÈS DE L'ÉCHANTILLON]`

**Observations qualitatives** : ______
**Déviations et observations** : ______

### 2.1.5 Critère de décision en fin de Série B

- Si le squeeze-out est **éliminé** par la seule pression réduite → la Série C teste alors si le confinement permet de *remonter* en pression (consolidation améliorée). Documenter ce pivot.
- Si le squeeze-out est **réduit mais présent** (cas attendu) → Série C telle que planifiée.
- Si le squeeze-out est **inchangé** → consigner, vérifier la mesure réelle de pression, puis Série C telle que planifiée.

---

## 2.2 SÉRIE C — Validation du confinement latéral (n = 3)

### 2.2.1 Objectif

Valider que l'ajout de parois de céramique en confinement latéral mécanique bloque physiquement le squeeze-out et le fiber flow, à pression et paramètres de chauffe identiques à la Série B.

### 2.2.2 Paramètres

Tous identiques à la Série B (courant, pression, profil, durée, empilement, film, gap), **plus** :

| Paramètre | Valeur |
|---|---|
| Parois de confinement | Blocs de céramique, matériau : ______ (recommandé : même famille que la céramique d'espacement — alumine / Macor — pour neutralité EM) |
| Nombre / position des parois | ______ (2 parois sur les bords longs ? 4 côtés ? — à fixer avant C-1) |
| Hauteur des parois | ______ mm (≥ épaisseur du stack laminés + film) |
| Fixation des parois | ______ (bridage ? rainure dans le support ? cales ?) |

### 2.2.3 Procédure de montage — confinement latéral (étape critique)

1. **Mesure préalable des laminés** : mesurer la largeur réelle du stack assemblé au pied à coulisse en 3 points le long du joint : ______ / ______ / ______ mm. Consigner la valeur max.
2. **Mesure de l'entrefer céramique** : mesurer l'écartement intérieur entre les parois de céramique montées, en 3 points : ______ / ______ / ______ mm.
3. **Calcul et consignation du jeu de tolérance** :

   > **Jeu latéral (par côté) = (écartement intérieur − largeur max du stack) / 2 = ______ mm**

   Le jeu est un **paramètre d'essai à part entière** : trop serré → contrainte parasite sur les bords, risque de marquage ou de blocage thermique différentiel ; trop lâche → le squeeze-out s'échappe dans le jeu et le confinement est inopérant. Valeur cible initiale suggérée : ______ mm (à fixer avant C-1, à consigner, et à garder identique sur C-1/C-2/C-3 sauf décision documentée).
4. **Alignement** :
   - Centrer le stack entre les parois (jeu symétrique gauche/droite, vérifié aux cales d'épaisseur : ______ mm chaque côté).
   - Vérifier le parallélisme parois / bords du laminé (écart < ______ mm sur la longueur).
   - Vérifier que les parois ne touchent **ni** la céramique d'espacement **ni** le concentrateur (jeu vertical : ______ mm) — la pression doit passer uniquement par le stack.
5. **Vérification EM** : noter la distance minimale parois–bobine : ______ mm. Au premier essai C-1, surveiller toute anomalie de chauffe (asymétrie IR, point chaud sur paroi). Consigner : ______
6. **Photo du montage confiné avant chauffe** (standard §2.2.5).
7. Dérouler ensuite les étapes 4 → 9 de la procédure Série B à l'identique.
8. **Post-essai spécifique C** : inspecter et photographier les faces internes des parois céramique (traces de matrice = preuve directe de squeeze-out intercepté). Mesurer la matrice déposée sur les parois si présente : ______

### 2.2.4 Fiches d'essai C-1, C-2, C-3

Structure identique aux fiches B, avec champs additionnels :

| Champ additionnel | Valeur |
|---|---|
| Jeu latéral consigné (gauche / droite) | ______ / ______ mm |
| Distance parois–bobine | ______ mm |
| Anomalie de chauffe liée aux parois | oui / non — détail : ______ |
| Matrice interceptée sur parois | oui / non — étendue : ______ |

`[INSÉRER COURBE DE CYCLE DE SOUDAGE — température, courant ET pression vs temps]`
`[INSÉRER PHOTO DU MONTAGE CONFINÉ AVANT CHAUFFE — vue de dessus + vue de côté]`
`[INSÉRER PHOTOS MACRO AVANT/APRÈS DE L'ÉCHANTILLON]`
`[INSÉRER PHOTOS DES FACES INTERNES DES PAROIS CÉRAMIQUE APRÈS ESSAI]`

### 2.2.5 Standardisation de la prise de photos (toutes séries)

| Règle | Spécification |
|---|---|
| Moments | (1) laminés nus avant empilement ; (2) montage complet avant chauffe ; (3) échantillon immédiatement après démontage ; (4) après refroidissement complet |
| Vues | Dessus + les deux côtés longs (zones de squeeze-out) + une vue 3/4 |
| Distance / cadrage | Fixe — utiliser un gabarit ou trépied repéré au marbre : distance ______ cm |
| Échelle | Réglet ou cale étalon **dans chaque photo** |
| Éclairage | Identique pour toute la campagne (noter la config : ______) |
| Nommage fichiers | `<ID essai>_<moment>_<vue>.jpg` (ex. `C-2_post_cote-gauche.jpg`) |

---

# 3. GRILLE DE MÉTRIQUES DE COMPARAISON (toutes séries)

À relever **après chaque essai**, méthode identique pour A, B et C.

## 3.1 Métriques primaires — sévérité du défaut

| # | Métrique | Méthode | Unité |
|---|---|---|---|
| M1 | Largeur max du bourrelet de squeeze-out (chaque côté) | Pied à coulisse / photo calibrée, 3 points par côté, max retenu | mm |
| M2 | Épaisseur résiduelle du pli twill au centre du joint | Micrographie, plan de coupe standardisé (voir §3.3) | µm |
| M3 | Perte d'épaisseur locale du joint = (épaisseur nominale − épaisseur min mesurée) / nominale | Micromètre, 5 points sur le joint | % |
| M4 | Angle de waviness max des fibres du twill | Micrographie, mesure d'angle | ° |
| M5 | Masse de matrice expulsée (si récupérable) ou masse échantillon avant/après | Balance ______ mg | mg |

## 3.2 Métriques secondaires — qualité du soudage

⚠️ La mitigation ne doit pas dégrader la chauffe interfaciale — sans ces métriques, la Série C ne valide rien.

| # | Métrique | Méthode | Unité |
|---|---|---|---|
| M6 | T max à l'interface | Thermocouple interface | °C |
| M7 | Temps au-dessus de T fusion PEKK (~337 °C) à l'interface | Courbe de cycle | s |
| M8 | Qualité d'interface (qualitatif → quantitatif) | Micrographie d'interface : porosités, continuité du film | classement 1–5 + % porosité si mesurable |
| M9 | (Optionnel, si éprouvettes disponibles) Résistance au cisaillement LSS | Essai single-lap shear | MPa |

## 3.3 Standardisation micrographie

- Plan de coupe : ______ (ex. transverse au joint, à mi-longueur) — **identique pour tous les échantillons, y compris les A déjà réalisés si re-découpe possible**.
- Grossissements : ______ × (vue d'ensemble) et ______ × (interface / twill).
- Polissage : protocole ______.

## 3.4 Tableau de synthèse final de campagne (à remplir au fil de l'eau)

| Essai | Courant (A) | Pression | Confinement | M1 (mm) | M2 (µm) | M3 (%) | M4 (°) | M6 (°C) | M7 (s) | M8 |
|---|---|---|---|---|---|---|---|---|---|---|
| A-1 | 250 | réf. | non | | | | | | | |
| A-2 | 250 | réf. | non | | | | | | | |
| A-3 | 200 | réf. | non | | | | | | | |
| B-1 | | réduite | non | | | | | | | |
| B-2 | | réduite | non | | | | | | | |
| B-3 | | réduite | non | | | | | | | |
| C-1 | | réduite | **oui** | | | | | | | |
| C-2 | | réduite | **oui** | | | | | | | |
| C-3 | | réduite | **oui** | | | | | | | |

---

# 4. Journal des déviations et décisions de campagne

| Date | Essai concerné | Déviation / décision | Justification | Impact sur comparabilité |
|---|---|---|---|---|
| | | | | |

---

*Document généré avec assistance IA (Claude) — structure et protocole à valider par l'étudiant et le directeur de recherche avant exécution. Les valeurs chiffrées suggérées (n=3, températures PEKK) sont indicatives et à confirmer selon les fiches matière et les capacités du banc.*
