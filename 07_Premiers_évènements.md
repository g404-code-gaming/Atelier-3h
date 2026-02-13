# 🎬 Découvrir l’onglet Événements

Jusqu’ici, on a ajouté des objets et des comportements.  
Maintenant, on va leur dire **quoi faire et quand le faire** 👇

---

## 🤔 Quel est le rôle de l’onglet Événements ?

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/38_Onglet_evenements.png" alt="Évènement" width="600"/>

L’onglet **Événements** est le cerveau de ton jeu 🧠

C’est ici que tu définis :

- ✅ Des **conditions** (quand quelque chose se passe)
- ⚡ Des **actions** (alors on fait quelque chose)

La logique fonctionne comme ça :

> **SI** une condition est vraie  
> **ALORS** on exécute une action

Exemple :
> SI la touche gauche est pressée  
> ALORS Dino marche

---

# ➕ Ajouter un premier événement

## 🎮 Événement 1 — Aller à gauche

1️⃣ Clique sur **Ajouter un événement**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/39_Evenements.png" alt="Évènement" width="600"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/40_Ajout_evenement.png" alt="Évènement" width="600"/>

### ➜ Condition

2️⃣ Clique sur **Ajouter une condition**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/41_Ajout_condition.png" alt="Évènement" width="600"/>

- Choisir à gauche : **Touche pressée**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/42_Touche.png" alt="Évènement" width="600"/>

- Sélectionner à droite : **Left (flèche gauche)**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/43_Left.png" alt="Évènement" width="600"/>  

- Valider par **OK**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/44_Ok.png" alt="Évènement" width="600"/>

On obtient notre **condition** :

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/45_Condition.png" alt="Évènement" width="600"/>

### ➜ Actions

En face de notre première condition, nous allons cliquer sur **Ajouter une action** :

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/46_Action.png" alt="Évènement" width="600"/>

- Nous allons **changer l’animation de Dino**
- Nom de l’animation : `walk`

*À gauche, nous cliquons sur notre personnage*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/47_Action_Dino.png" alt="Évènement" width="600"/>

*Au centre, nous cliquons sur Animation (par nom)*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/48_Animation_nom.png" alt="Évènement" width="600"/>

*À droite, nous cliquons sur la liste d'animation*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/49_Liste.png" alt="Évènement" width="600"/>

*Nous sélectionnons Walk*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/50_Walk.png" alt="Évènement" width="600"/>

*On valide avec Ok*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/52_Ok.png" alt="Évènement" width="600"/>

Nous obtenons notre **action** :  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/53_Action.png" alt="Évènement" width="600"/>

Ajouter une seconde action :

- **Inverser l’objet horizontalement**
- Mettre sur : **Oui**

*À gauche, nous cliquons sur notre personnage*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/47_Action_Dino.png" alt="Évènement" width="600"/>

*Au centre, nous cliquons sur Inverser l'affichage de l'objet horizontalement*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/54_Inverser.png" alt="Évènement" width="600"/>

*À droite, nous cliquons sur Oui*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/55_Oui.png" alt="Évènement" width="600"/>

👉 Dino regarde vers la gauche quand il marche à gauche.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/57_Actions.png" alt="Évènement" width="600"/>

---

## 🎮 Événement 2 — Aller à droite

1️⃣ Clique sur **Ajouter un événement**

### ➜ Condition

- À gauche, nous sélectionnons à nouveau **Touche pressée**
- Sélectionner au milieu : **Right (flèche droite)**
- Valider avec **Ok**

### ➜ Actions

1️⃣ **Changer l’animation de Dino**
- Cliquer sur **Ajouter une action**
- Cliquer à gauche sur **Dino** puis au milieu sur **Animation (par nom)**
- Nom de l'animation : `walk`

2️⃣ **Inverser l’objet horizontalement**
- Ajouter une seconde action
- Cliquer à gauche sur **Dino** puis au milieu sur **Inverser l'affichage de l'objet horizontalement**
- Mettre sur : **Non**

👉 Dino regarde vers la droite quand il marche à droite.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/58_Droite.png" alt="Évènement" width="600"/>

---

## 🎮 Événement 3 — Revenir en Idle

1️⃣ Ajouter un nouvel événement

### ➜ Condition

- **N’importe quelle touche est relâchée**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/59_Relacher.png" alt="Évènement" width="600"/>

### ➜ Action

- **Changer l’animation de Dino**
- Nom : `Idle`

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/60_Idle.png" alt="Évènement" width="600"/>

👉 Quand on relâche les touches, Dino arrête de marcher et revient en animation d’attente.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/61_Action.png" alt="Évènement" width="600"/>

---

### Sauvegarder

Pensez à sauvegarder votre projet en cliquant sur la **disquette**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/19_Sauvegarder.png" alt="Évènement" width="600"/>

---

# ✅ Résultat

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/62_Scene.png" alt="Évènement" width="600"/>

- Dino marche vers la gauche
- Dino marche vers la droite
- Dino se retourne selon la direction
- Dino revient en position Idle quand on arrête d’appuyer

🎉 Le déplacement devient beaucoup plus réaliste !

Ton jeu commence vraiment à prendre vie 🔥
