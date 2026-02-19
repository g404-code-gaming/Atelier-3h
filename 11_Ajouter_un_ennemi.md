# 👾 Ajouter un ennemi

## ➕ Ajouter l’ennemi

- Ajoute un objet (ex: **Zombie Boy**)  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/111_Zombie.png" alt="Ennemi" width="600"/>

- Place-le sur une plateforme

Pour l’instant, il ne bouge pas.

---

## 💀 Collision Dino / Ennemi

### Cas 1 : Dino touche l’ennemi au sol

Crée un événement :

#### ➜ Conditions
- Première condition : il faut gérer la collision de **Dino** avec **Zombie Boy**
- Pour cela, **Ajoute un condition**, clique sur ton *Dino* à gauche, choisis *Collision* dans les actions et choisis *Zombie Boy* à droite  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/112_Collision_zombie.png" alt="Ennemi" width="900"/>

- Seconde condition : **Dino** doit être sur le *sol*
- Pour cela, ajoute une seconde condition, clique sur Dino et trouve l'action **Est sur le sol**  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/113_Sol.png" alt="Ennemi" width="400"/>

#### ➜ Actions
Pour les actions à ajouter, tu commences à les connaître. Il faut:  
- Changer l'**Animation (par nom)** de Dino à `Dead`
- Attendre 2 secondes
- Changer la scène e relancer *Scène sans titre* dans les **Autres actions**  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/114_Animation_dead.png" alt="Ennemi" width="900"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/115_Code_dead.png" alt="Ennemi" width="900"/>

---

### Cas 2 : Dino saute sur l’ennemi

Crée un autre événement :

#### ➜ Conditions
La collision de **Dino** avec **Zombie Boy** est la même qu'au-dessus.  
Ce qui change, c'est que Dino retombe d'un saut.  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/112_Collision_zombie.png" alt="Ennemi" width="900"/>

Ajoute comme seconde condition : *Dino* est **En train de tomber**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/116_Tomber.png" alt="Ennemi" width="500"/>

#### ➜ Action
- Supprime *Zombie Boy*  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/117_Code_tomber.png" alt="Ennemi" width="900"/>

👉 Comme dans un vrai jeu de plateforme 😉

---

### Sauvegarder

Pense à sauvegarder ton projet en cliquant sur la **disquette**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/19_Sauvegarder.png" alt="Évènement" width="400"/>
