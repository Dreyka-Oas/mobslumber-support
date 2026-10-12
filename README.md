# MobSlumber support

English first, français plus bas.

MobSlumber is a Fabric mod that slows down the brain and the pathing of every mob as it gets farther from a player. Each mob falls into a tier by its distance to the nearest player: active, reduced, drowsy or asleep. The radius is set per category, and a mob that is close is never touched. Mobs that are asleep and standing still can skip a whole tick between two full ones. Settings and presets let you choose how far to push it. It needs ComputeTide and OasCore.

This repository holds no code. It is the place to report a problem or ask a question about the mod, and nothing else.

## Reporting a bug

Open an issue and pick the bug form. It asks for the game and loader versions, the mod version, what you expected, what happened, the steps to reproduce it and the lines of `latest.log` around it. A report with those lines gets answered much faster than one without them.

Before you write, run `/mobslumber status` on the server. It shows how many loaded mobs sit in each tier, whether the server is under load, how many whole ticks were skipped in the last second, which ComputeTide backend answers and how MobSlumber shares the work with the other optimisation mods it found. Settings live in OasCore, in the MobSlumber tab, and in `config/oas/mobslumber/mobslumber.json`. The server preset and the display preset can each be Light, Normal or Strong, and an option you changed by hand keeps its own value.

## What is not a bug

A mob far from every player that moves slowly, thinks rarely or stands still is the whole point of the mod. A mob that was hurt or woken stays fully active for a short while, and a mob close to a player always runs like the base game. Some mobs are exempt on purpose: the status line counts them. When another optimisation mod such as ServerCore, Immersive Optimization, Lithium or Entity Culling is installed, each one has a choice in the Other mods category, so check it before reporting a mob that seems frozen. If the client log says masking is off for the session, that is a ComputeTide ray failure being reported, and it does not stop the rest of the mod.

## Français

MobSlumber est un mod Fabric qui ralentit le cerveau et la recherche de chemin de chaque mob à mesure qu'il s'éloigne d'un joueur. Chaque mob tombe dans un palier selon sa distance au joueur le plus proche : actif, réduit, somnolent ou endormi. Le rayon se règle par catégorie, et un mob proche n'est jamais touché. Les mobs endormis et immobiles peuvent sauter un tour entier entre deux tours complets. Les réglages et les préréglages disent jusqu'où aller. Il demande ComputeTide et OasCore.

Ce dépôt ne contient aucun code. On y signale un problème ou on y pose une question sur le mod, rien d'autre.

### Signaler un bug

Ouvrez un ticket et choisissez le formulaire de bug. Il demande les versions du jeu et du chargeur, la version du mod, ce que vous attendiez, ce qui s'est passé, les étapes pour le reproduire et les lignes de `latest.log` autour du problème. Un signalement avec ces lignes reçoit une réponse bien plus vite.

Avant d'écrire, lancez `/mobslumber status` sur le serveur. La commande montre combien de mobs chargés se trouvent dans chaque palier, si le serveur est sous charge, combien de tours entiers ont été sautés pendant la dernière seconde, quel moteur de ComputeTide répond et comment MobSlumber partage le travail avec les autres mods d'optimisation qu'il a trouvés. Les réglages sont dans OasCore, onglet MobSlumber, et dans `config/oas/mobslumber/mobslumber.json`. Le préréglage du serveur et celui de l'affichage valent chacun Léger, Normal ou Fort, et une option changée à la main garde sa propre valeur.

### Ce qui n'est pas un bug

Un mob loin de tous les joueurs qui bouge doucement, réfléchit rarement ou reste immobile, c'est le but du mod. Un mob blessé ou réveillé reste pleinement actif un court moment, et un mob proche d'un joueur tourne toujours comme dans le jeu de base. Certains mobs sont exemptés exprès : la ligne de statut les compte. Quand un autre mod d'optimisation comme ServerCore, Immersive Optimization, Lithium ou Entity Culling est installé, chacun a son choix dans la catégorie Other mods, alors regardez-le avant de signaler un mob qui semble figé. Si le journal du client dit que le masquage est coupé pour la session, c'est une panne des rayons de ComputeTide qui est signalée, et le reste du mod continue de tourner.
