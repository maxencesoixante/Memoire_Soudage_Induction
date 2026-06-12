# Cahier de laboratoire — Campagne de soudage par induction semi-statique

**Projet** : Mitigation du fiber flow / squeeze-out en soudage par induction semi-statique de laminés CF-PEKK
**Configuration** : Pression de consolidation transmise par le concentrateur de flux via céramique d'espacement
**Auteur** : Maxence Dubois
**Institution** : ÉTS — Montréal
**Période de la campagne** : 11 / 06 / 2026 → ?? / ?? / 2027
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

| Élément | Spécification                                                                                                                                                                             |
|---|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Laminé supérieur | CF-PEKK, empilement [45/-45/0/90]₃ₛ + **pli twill sur la surface supérieure mais positionné à l'interface de soudure** (couche suscepteur, maximisation de la chauffe par courants de Foucault) |
| Laminé inférieur | CF-PEKK, empilement [45/-45/0/90]₃ₛ                                                                                                                                                       |
| Interface de soudage | Film PEKK, épaisseur 0,004 po (~0,10 mm)                                                                                                                                                  |
| Dimensions laminés | 120 × 40 × 3,36 mm                                                                                                                                                           |
| Recouvrement (overlap) | 120 x 40 mm                                                                                                                                                                               |
| Lot matière / traçabilité | ????                                                                                                                                                                                      |

### 1.2.2 Chaîne de transmission de la pression

```text
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