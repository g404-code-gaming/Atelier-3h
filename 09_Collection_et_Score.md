# 📊 Gérer un score

## 📊 Créer une variable Score

1️⃣ Ouvre l’onglet **Événements**  
2️⃣ Clique sur *Ajouter une condition*
3️⃣ Ajoute une action au début de la scène dans **Autres conditions** puis **Au lancement de la scène** :

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/65_Autres_conditions.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/66_Lancement.png" alt="Score" width="700"/>

- **Au début de la scène**
  - Action → Modifier une variable de scène dans **Autres actions**
  - Clique à gauche sur **Variables** puis *Changer la valeur de la variable*
  - Clique à droite sur **+ Ajouter ou modifier des variables**
  - Nom à entrer : `Score`
  - Valeur à définir : `0`
  - Clique sur Ok ou Appliquer

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/67_Changer_variable.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/68_Ajout_variable.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/69_Score.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/70_Valeur_0.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/71_Initialisation.png" alt="Score" width="700"/>

---

## 🏆 Gérer la collecte

Crée un nouvel événement :

### ➜ Condition
- Dino est en collision avec ChickenLeg
- Clique sur **Dino** à gauche
- Au milleu, clique sur **Collision**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/72_Collision.png" alt="Score" width="700"/>

- À droite, choisis l'objet **chicken leg**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/73_Choix_objet.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/74_Chicken_leg.png" alt="Score" width="700"/>

### ➜ Actions
- Clique sur **Autres actions** puis **Variables** puis *Changer la valeur de la variable*
- Ajoute **1** à la variable `Score`

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/75_Ajout_score.png" alt="Score" width="700"/>

- Supprime l’objet ChickenLeg

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/76_Objet_chicken.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/77_Supprimer.png" alt="Score" width="700"/>

👉 À chaque contact, on gagne un point et l’objet disparaît.

---

# 🖥️ Afficher le score (UI fixe)

## ➕ Ajouter un objet Texte

1️⃣ Ajouter un nouvel objet → **Texte**
2️⃣ Nommer l’objet : `ScoreText`
3️⃣ Le placer en haut à gauche de la scène

---

## 📌 Le mettre sur un calque UI

1️⃣ Créer un nouveau **calque**
2️⃣ Nommer le calque : `UI`
3️⃣ Placer `ScoreText` sur ce calque

👉 Un calque UI ne bouge pas avec la caméra.

---

## 🔄 Mettre le texte à jour dynamiquement

Créer un événement :

### ➜ Condition
- Toujours (aucune condition)

### ➜ Action
- Modifier le texte de ScoreText :
  
"Score : " + ToString(Score)


👉 Le score s’affiche en temps réel.
