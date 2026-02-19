# 👾 Bonus final : Faire patrouiller l’ennemi (version détaillée)

On va maintenant rendre ton ennemi un peu plus intelligent 😈  
Tu vas lui faire faire des allers-retours sur sa plateforme, comme dans un vrai jeu de plateforme.

L’idée est simple :

- Tu définis une direction (`left` ou `right`)
- Tu appliques une force selon cette direction
- Tu changes la direction quand il touche une limite invisible

---

# 🏁 1️⃣ Ajouter des limites invisibles

Pour que ton ennemi sache où s’arrêter, tu dois placer deux repères invisibles.

## ➕ Crée les objets limites

1️⃣ Clique sur **Ajouter un nouvel objet**  dans le *Magasin de ressources*  
2️⃣ Choisis les objets **Right_arrow_round_button** et **Left_arrow_round_button**   
3️⃣ Ajoute-les à la scène  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/141_Ajout_fleche.png" alt="Ennemi" width="800"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/142_Ajout_fleche.png" alt="Ennemi" width="800"/>

---

## 👻 Rends-les invisibles

Tu ne veux pas que le joueur voie ces blocs. On va donc les **cacher** au lancement de la scène.  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/144_Cacher.png" alt="Ennemi" width="800"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/145_Code_cacher.png" alt="Ennemi" width="800"/>

---

## 📍 Place-les correctement

Dans la scène, place les objets *flèches* autour de la plateforme de l'ennemi comme sur le schèma suivant - **Zombie_Boy** devra se trouver entre ces deux limites.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/143_Placement.png" alt="Ennemi" width="800"/>

---

# 🔁 2️⃣ Ajouter une variable de direction

Maintenant, tu vas donner une information à ton ennemi : sa direction actuelle.

1️⃣ Double-clique à droite sur l’objet **Zombie_Boy**  
2️⃣ Va dans l'onglet **Variables**
3️⃣ Ajoute une variable d’objet `direction` qui est un texte et met *"right"* en valeur  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/146_Variable_direction.png" alt="Ennemi" width="800"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/147_Options_variable.png" alt="Ennemi" width="800"/>

Ajoute ensuite dans le bloc *Au lancement de la scène* l'action de la variable comme suit : 

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/152_Depart.png" alt="Ennemi" width="800"/>

Au départ, ton ennemi partira vers la droite.

Cette variable contiendra toujours soit `"right"` soit `"left"`.

---

# 💨 3️⃣ Déplacer l’ennemi selon sa direction

Tu vas maintenant créer les événements qui le font avancer.

---

## ➜ S’il va vers la droite

Crée un nouvel événement.

### Conditions

Dans Autres condition, change la valeur de la variable de **Zombie_Boy** `direction` à `"right"`  

### Action

Dans Ajouter une action, cherche *Appliquer une force (avec angle)*  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/149_Force.png" alt="Ennemi" width="500"/>

- Ajoute une force à **Zombie_Boy**
  - Angle : 0° (vers la droite)
  - Vitesse : 100px
  - Instantané : Oui
 
  <img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/150_Options_force.png" alt="Ennemi" width="500"/>

Ainsi, tant que la variable vaut `"right"`, ton ennemi avance vers la droite.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/148_Condition_variable.png" alt="Ennemi" width="800"/>

---

## ➜ S’il va vers la gauche

Crée un second événement.

### Conditions

Dans Autres condition, change la valeur de la variable de **Zombie_Boy** `direction` à `"left"` 

### Action

Dans Ajouter une action, cherche *Appliquer une force (avec angle)*  

- Ajoute une force à Enemy
  - Angle : 180° (vers la gauche)
  - Vitesse : 100
  - Instantané : Oui

Ton ennemi avance maintenant vers la gauche quand la variable change.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/151_Forces.png" alt="Ennemi" width="800"/>

---

# 🔄 4️⃣ Changer de direction aux limites

Maintenant, tu vas lui apprendre à se retourner.

---

## ➜ Quand il touche la flèche à droite

Crée un événement :

### Conditions

- Collision entre **Zombie_boy** et **Left_arrow_round_button**

### Actions

- Modifie la variable `direction` = `"left"`  
- Inverse horizontalement l’ennemi = Oui  
- Ajoute l'animation par nom de **Zombie_Boy** à `Walk`  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/154_Left.png" alt="Ennemi" width="800"/>

Dès qu’il touche la limite droite, il repart vers la gauche.

---

## ➜ Quand il touche la limite gauche

Crée un autre événement :

### Conditions

- Collision entre **Zombie_boy** et **Right_arrow_round_button**


### Actions

- Modifie la variable `direction` = `"right"`  
- Inverse horizontalement l’ennemi = Non  
- - Ajoute l'animation par nom de **Zombie_Boy** à `Walk`  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/155_Right.png" alt="Ennemi" width="800"/>

Il repart alors vers la droite.

---



# 🎯 Ce que tu viens de faire

Tu as créé :

- Une variable qui stocke un état
- Un déplacement conditionnel
- Un système de patrouille automatique
- Un changement de direction basé sur des collisions

Ton ennemi ne reste plus immobile.  
Il surveille sa plateforme comme un vrai garde 👾🔥

---

# 🎉 Félicitations

Tu viens de créer un vrai petit jeu de plateforme complet.  
Bravo à toi 👏🔥
