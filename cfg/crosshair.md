# 🎯 Crosshair — by.jkz

## Pourquoi pas de code de partage CS2 ?

Les codes de partage CS2 ne sont pas toujours fidèles aux valeurs exactes enregistrées dans les fichiers Steam. Les commandes console ci-dessous garantissent un résultat 100% identique à la config réelle.

---

## Paramètres

| Paramètre | Valeur |
|---|---|
| Style | **2** — Statique classique |
| Taille | **1.5** |
| Gap | **+2** |
| Épaisseur | **2** |
| Point central | **Non** |
| Contour | **Oui** |
| Couleur | **Cyan** (R:50 G:255 B:255) |
| Alpha | **255** (opaque) |
| T-shape | **Non** |
| Recoil dynamique | **Non** |

---

## Commandes console — Copier-coller dans CS2

Ouvre la console CS2 (touche ` ` `) et colle ces commandes :

```
cl_crosshairstyle 2
cl_crosshairsize 1.5
cl_crosshair_thickness 2
cl_crosshair_gap 2
cl_crosshairdot false
cl_crosshair_drawoutline true
cl_crosshaircolor_r 50
cl_crosshaircolor_g 255
cl_crosshaircolor_b 255
cl_crosshairalpha 255
cl_crosshair_t false
cl_crosshair_recoil false
```

> Ces paramètres sont stockés dans `cfg/cs2_user_convars_0_slot0.vcfg` et se chargent automatiquement via Steam Cloud.

---

## Pourquoi ce crosshair ?

- **Style 2 statique** — ne bouge pas pendant le mouvement, idéal pour le placement de crosshair conscient
- **Gap +2** — crosshair serré sans être collé, bon équilibre précision/lisibilité
- **Épaisseur 2** — bien visible sans être encombrant
- **Cyan (R:50 G:255 B:255)** — haute visibilité sur tous les environnements de maps compétitives
- **Contour activé** — reste lisible sur les fonds clairs (ciel, murs blancs)
- **Recoil false** — crosshair fixe, le spray control est appris manuellement
