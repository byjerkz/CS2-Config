# 📦 Guide d'installation complet

## Prérequis

- Counter-Strike 2 installé via Steam
- Ton Steam ID (voir ci-dessous comment le trouver)

---

## 🔍 Trouver ton Steam ID

1. Ouvre Steam
2. Clique sur ton profil en haut à droite
3. Clique sur **"Détails du compte"**
4. Ton Steam ID est affiché sous ton nom (ex: `123456789`)

Ou via l'URL de ton profil Steam :  
`https://steamcommunity.com/profiles/76561198XXXXXXXXX`  
→ Les 17 derniers chiffres = ton SteamID64  
→ Pour le dossier userdata, utilise le nombre après `/userdata/` dans l'explorateur

---

## 📁 Étape 1 — autoexec.cfg

Copie `autoexec.cfg` dans :
```
C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg\
```

---

## 📁 Étape 2 — cs2_video.txt

Copie `cs2_video.txt` dans :
```
C:\Program Files (x86)\Steam\userdata\[TON_STEAM_ID]\730\local\cfg\
```
Remplace `[TON_STEAM_ID]` par ton propre Steam ID.

### ⚠️ Important — Mettre en lecture seule
Après avoir copié le fichier :
1. Clic droit sur `cs2_video.txt`
2. Propriétés
3. Cocher **Lecture seule**
4. OK

Sans ça, CS2 réécrit le fichier à chaque modification dans les options graphiques.

---

## 📁 Étape 3 — Fichiers cfg/ (optionnel mais recommandé)

Ces fichiers garantissent le crosshair, la sensibilité et les binds même si l'autoexec est chargé après.

Copie les deux fichiers du dossier `cfg/` dans :
```
C:\Program Files (x86)\Steam\userdata\[TON_STEAM_ID]\730\local\cfg\
```

---

## 🚀 Étape 4 — Options de lancement Steam

1. Clic droit sur **Counter-Strike 2** dans Steam
2. **Propriétés**
3. **Options de lancement**
4. Colle :
```
-novid +fps_max 240 +exec autoexec.cfg -allow_third_party_software -nojoy
```

> ⚠️ Adapte `fps_max` selon ton écran :
> - 120Hz → `+fps_max 240`
> - 144Hz → `+fps_max 288`
> - 240Hz → `+fps_max 480`
> - 360Hz → `+fps_max 720`
> - 500Hz+ → `+fps_max 0` (illimité)

---

## ✅ Étape 5 — Vérification

Lance CS2 → Ouvre la console (touche `` ` ``) → Tu dois voir :

```
###############################################################
#         🚀 CS2 PRO LOW LATENCY CONFIG v4.0 - LOADED        #
#                    👨‍💻  by.jkz                              #
###############################################################
```

Si tu vois ce message, la config est chargée correctement.

---

## 🌐 Wi-Fi vs Filaire

Dans `autoexec.cfg`, ligne `cl_net_buffer_ticks` :
- **Wi-Fi** → `cl_net_buffer_ticks 2` (défaut dans cette config)
- **Filaire** → `cl_net_buffer_ticks 1`

Modifie selon ta connexion.

---

## ❓ Problèmes fréquents

**La config ne se charge pas**
→ Vérifie que `autoexec.cfg` est bien dans le dossier `cfg\` et que l'option de lancement `+exec autoexec.cfg` est présente.

**La résolution ne change pas**
→ Vérifie que `cs2_video.txt` est en lecture seule et au bon emplacement.

**Les binds ne fonctionnent pas**
→ Copie les fichiers `.vcfg` du dossier `cfg/` dans le dossier userdata Steam.
