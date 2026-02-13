# ⚙️ Ajouter des comportements aux objets

Maintenant que notre scène est prête, on va donner des **capacités** à nos objets 🎮

---

## 🤔 C’est quoi un comportement ?

Un **comportement** permet d’ajouter des fonctionnalités automatiques à un objet,  
sans avoir besoin d’écrire d’événements compliqués.

En gros :
- L’objet sait **comment se comporter tout seul**
- On lui donne un rôle (personnage, plateforme, caméra, etc.)

Exemples :
- Un comportement *Personnage plateforme* permet de marcher et sauter
- Un comportement *Plateforme* permet d’être solide
- Un comportement *Caméra* permet de suivre un objet

---

## 🦖 Ajouter des comportements à Dino

1️⃣ Dans la liste des objets à droite, **double-clique sur Dino**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/20_Options_dino.png" alt="Comportements" width="700"/>

2️⃣ Clique sur **"Ajouter un comportement"**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/21_Onglet_comprtements.png" alt="Comportements" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/22_Ajout_comportement.png" alt="Comportements" width="700"/>

### ➜ Ajouter le comportement **Personnage plateforme**

- Sélectionne **Personnage plateforme**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/23_Comportements.png" alt="Comportements" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/24_Personnage.png" alt="Comportements" width="700"/>

- Laisse les options de base sans rien toucher

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/25_Options_base.png" alt="Comportements" width="700"/>

- Valide avec le bouton **Appliquer**

👉 Dino peut maintenant marcher et sauter (une fois les contrôles activés).

---

### ➜ Ajouter le comportement **Caméra fluide**

- Clique à nouveau sur **"Ajouter un comportement"** en bas à droite
- Choisis **Caméra fluide**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/26_Camera_fluide.png" alt="Comportements" width="700"/>

Ensuite :

- Dans les paramètres du comportement,
- Décoche **"Follow on Y axis"**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/27_Options_camera.png" alt="Comportements" width="700"/>

- Valide en cliquant sur **Appliquer**

👉 La caméra suivra Dino seulement horizontalement  
👉 Elle ne montera pas quand il saute (plus confortable pour un jeu plateforme).

---

## 🧱 Ajouter le comportement Plateforme

Maintenant, on doit rendre nos plateformes… solides 😄

Pour chaque plateforme :

1️⃣ Double-clique sur la plateforme dans la liste à droite  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/28_Plateforme_options.png" alt="Comportements" width="700"/>

2️⃣ Clique sur **"Ajouter un comportement"**  
3️⃣ Choisis **Plateforme**  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/29_Comportement_plateforme.png" alt="Comportements" width="700"/>

4️⃣ Valide avec **Appliquer**

Répète l’opération pour toutes les plateformes.

---

## 🧱 Plateforme vs Plateforme franchissable

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/30_Options.png" alt="Comportements" width="700"/>

### 🔹 Plateforme classique
- Solide
- On ne peut pas la traverser
- On ne peut pas sauter à travers par dessous

👉 Parfait pour le sol principal.

---

### 🔹 Plateforme franchissable
- On peut **sauter à travers par dessous**
- Mais on atterrit dessus quand on vient d’en haut

👉 Idéal pour :
- Des plateformes suspendues
- Des étages
- Des éléments type Mario

---

## ▶️ Lancer l’aperçu

Clique sur **"Aperçu"** (bouton en haut de l’écran).

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/31_Apercu.png" alt="Comportements" width="500"/>

🎮 Teste ton jeu :

- ⬅️ ➡️ Flèches directionnelles → déplacer Dino
- ⬆️ ou Barre espace → sauter

---

## ✅ Résultat

- 🦖 Dino peut bouger
- 🎥 La caméra le suit
- 🧱 Les plateformes sont solides

Ton jeu commence officiellement à fonctionner 🔥

Nous allons maintenant améliorer les **collisions** entre le Dino et les plateformes.
