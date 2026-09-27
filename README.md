# 🎯 CS2 Config — by JKZ

> Setup compétitif CS2 | FACEIT | Low Latency  
> 800 DPI · sens 1.25 · eDPI 1000 · 1280×960 4:3 · 120Hz

---

## 📁 Structure

```
CS2-Config/
├── autoexec.cfg                          # Config principale (exécutée au lancement)
├── cs2_video.txt                         # Paramètres vidéo
├── .gitignore
├── .gitattributes
├── LICENSE
├── cfg/
│   ├── cs2_user_convars_0_slot0.vcfg     # Réglages utilisateur (crosshair, souris, viewmodel)
│   ├── cs2_user_keys_0_slot0.vcfg        # Binds clavier/souris
│   ├── cs2_machine_convars.vcfg          # Réglages machine (réseau, audio, HUD)
│   └── M36HE-CS2.json                    # Profil clavier Attack Shark M36HE
└── docs/
    ├── installation.md
    ├── hardware.md
    └── crosshair.md
```

---

## 🖱️ Souris

| Paramètre | Valeur |
|-----------|--------|
| DPI | 800 |
| Sensibilité CS2 | 1.25 |
| eDPI | **1000** |
| m_pitch | 0.022 |
| m_yaw | 0.022 |
| zoom_sensitivity_ratio | 1 |
| sensitivity_y_scale | 1 |

---

## ✳️ Crosshair

| Paramètre | Valeur |
|-----------|--------|
| Style | 2 (Classique statique) |
| Couleur | Cyan (R:50 G:255 B:255) |
| Alpha | 255 |
| Gap | +2 |
| Length | 4 |
| Thickness | 2 |
| Size | 1.5 |
| Dot | OFF |
| Outline | ON |
| T-shape | OFF |
| Recoil | OFF |

**Share code** : `CSGO-XXXXX` *(générer via le jeu)*

---

## 🔫 Viewmodel

| Paramètre | Valeur |
|-----------|--------|
| viewmodel_fov | 68 |
| viewmodel_offset_x | 2.5 |
| viewmodel_offset_y | 0 |
| viewmodel_offset_z | -1.5 |
| Preset | 2 (Compétitif) |

---

## 🖥️ Vidéo

| Paramètre | Valeur |
|-----------|--------|
| Résolution | 1280×960 |
| Ratio | 4:3 |
| Mode | Plein écran |
| Refresh rate | 120Hz |
| VSync | OFF |
| Low Latency | OFF |
| MSAA | OFF |
| Shadows | ON |
| HDR Detail | 3 |

---

## ⚡ Réseau & Performance

| Paramètre | Valeur |
|-----------|--------|
| rate | 786432 |
| cl_net_buffer_ticks | 1 (filaire) / 2 (Wi-Fi) |
| mm_dedicated_search_maxping | 25ms |
| fps_max | 240 |

> ⚠️ Le fichier `cs2_machine_convars.vcfg` est actuellement configuré avec `cl_net_buffer_ticks 2` (mode Wi-Fi).  
> Passe à `1` si tu joues en filaire.

---

## 🎧 Audio

| Paramètre | Valeur |
|-----------|--------|
| snd_headphone_eq | 1 (EQ Valve désactivé) |
| snd_spatialize_lerp | 0.8 |
| snd_mixahead | 0.011 |
| Musiques (menu/MVP/round) | OFF |
| Volume vocal équipe | 0.3 |
| snd_tensecondwarning_volume | 0.05 |

---

## ⌨️ Binds principaux

| Touche | Action |
|--------|--------|
| SHIFT | Drop arme secondaire |
| G | Drop bombe |
| 1 | HE Grenade (slot6) |
| 2 | Flashbang (slot7) |
| 3 | Smoke (slot9) |
| 4 | Molotov/Incendiaire (slot8) |
| 5 | Decoy (slot10) |
| SPACE | Jump |
| CTRL | Équiper bombe (slot5) |
| MOUSE4 | Duck |
| MOUSE5 | Sprint |
| MWHEELUP | Arme principale |
| MWHEELDOWN | Arme secondaire |
| E | Couteau |
| F | Use / Ramasser |
| Q | Drop arme |
| X | Push to talk |
| T | Chat équipe |
| P | Reload autoexec |
| ` | Console |

---

## 🚀 Launch Options Steam

```
-novid +fps_max 240 +exec autoexec.cfg -allow_third_party_software -nojoy
```

---

## 🛠️ Installation

Voir [`docs/installation.md`](docs/installation.md) pour le guide complet.

---

## 💻 Hardware

| Composant | Modèle |
|-----------|--------|
| Clavier | Attack Shark M36HE (Hall Effect) |
| Setup | Voir [`docs/hardware.md`](docs/hardware.md) |

---

## 📝 Notes

- Config optimisée pour jeu **filaire** — adapter `cl_net_buffer_ticks` si Wi-Fi
- `fps_max 240` — adapter selon le Hz de ton écran
- Le profil clavier `cfg/M36HE-CS2.json` est importable directement dans le logiciel Attack Shark
