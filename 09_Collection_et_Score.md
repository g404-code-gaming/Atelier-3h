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
 
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/67_Changer_variable.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/68_Ajout_variable.png" alt="Score" width="700"/>

  - Clique à droite sur **+ Ajouter ou modifier des variables**
 
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/69_Score.png" alt="Score" width="700"/>

  - Nom à entrer : `Score`
  - Valeur à définir : `0`
  - Clique sur Ok ou Appliquer

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/70_Valeur_0.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/71_Initialisation.png" alt="Score" width="900"/>

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

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/67_Changer_variable.png" alt="Score" width="700"/>

- Ajoute **1** à la variable `Score`

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/75_Ajout_score.png" alt="Score" width="700"/>

- Supprime l’objet ChickenLeg

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/76_Objet_chicken.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/77_Supprimer.png" alt="Score" width="700"/>

👉 À chaque contact, on gagne un point et l’objet disparaît.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/78_Code.png" alt="Score" width="900"/>

---

# 🖥️ Afficher le score (UI fixe)

## ➕ Ajouter un objet Texte

1️⃣ Ajoute un nouvel objet → **Texte**  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/79_Nouvel_objet.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/80_Texte.png" alt="Score" width="700"/>

2️⃣ Nommerl’objet : `ScoreText`, met la taille de police à 40 et **Score:** en valeur  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/81_Options_texte.png" alt="Score" width="700"/>

3️⃣ Place le en haut à gauche de la scène  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/82_Placement_texte.png" alt="Score" width="700"/>

---

## 📌 Le mettre sur un calque UI

1️⃣ Crée un nouveau **calque** en cliquant sur l'icône `Calque` en haut à droite  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/83_Icone_calques.png" alt="Score" width="400"/>

2️⃣ Clique sur **+** et nomme le calque : `UI`  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/84_Ajout_calque.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/85_UI.png" alt="Score" width="700"/>

3️⃣ Place `ScoreText` sur ce calque à gauche dans les propriétés de l'objet sur la scène 

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/86_Selection_texte.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/87_Choix_calque.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/88_Calque_UI.png" alt="Score" width="700"/>

👉 Un calque UI ne bouge pas avec la caméra.

---

## 🔄 Mettre le texte à jour dynamiquement

Crée un événement :

### ➜ Condition
- Aucune condition - ce qui signifie que l'évènement a toujours lieu

### ➜ Action
- Clique sur l'objet `Texte` à gauche puis sur l'action `Texte`au milieu et modifie le texte de *ScoreText* et met la formule suivante :

```js  
"Score : " + ToString(Score)
```

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/89_Selection_objet_texte.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/90_Action_texte.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/91_Option_texte.png" alt="Score" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/92_Copie_code.png" alt="Score" width="700"/>

👉 Le score s’affiche en temps réel.
