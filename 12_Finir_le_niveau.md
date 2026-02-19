# 🏁 Finaliser l’atelier : gérer les scènes et la fin du jeu

On va maintenant structurer proprement notre jeu avec un **niveau 1** et un **écran de fin** 🎉

---

# 🎬 1️⃣ Renommer et organiser les scènes

## ✏️ Renommer la scène principale

1️⃣ Dans le gestionnaire de scènes (bouton Menu en haut à gauche)  
2️⃣ Clique droit sur **Scène sans titre**  
3️⃣ Renomme-la *niveau 1*. Ta scène va se fermer, c'est normal, tu as juste à double-cliquer sur *niveau 1* pour le rouvrir.  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/121_Ajout_scene.png" alt="fin" width="500"/>


---

## ➕ Ajouter une seconde scène

1️⃣ Clique sur **Ajouter une scène**  
2️⃣ Nomme-la *fin*

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/122_Ajout_scene_detail.png" alt="fin" width="500"/>

👉 Nous aurons donc :
- `niveau 1` → le jeu
- `fin` → l’écran de victoire

---

# 🚪 2️⃣ Ajouter la porte de fin

## ➕ Placer la porte

- Ajouter un objet **Porte** dans ton *niveau 1*  
- La placer sur une plateforme en fin de niveau

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/118_Porte.png" alt="fin" width="800"/>

---

## 🎯 Condition pour terminer le niveau

Dans les **événements de "niveau 1"**, ajoute :

### ➜ Conditions

- **Dino** est en collision avec **Porte**
- Change la valeur de la variable `Score` et définit la au nombre total de *Chicken Leg* du niveau

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/119_Collision_porte.png" alt="fin" width="800"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/120_Verification_score.png" alt="fin" width="800"/>

### ➜ Actions

- Attendre **1 seconde**
- Changer de scène → `fin`

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/123_Changer_scene.png" alt="fin" width="800"/>

👉 La porte ne fonctionne que si tous les objets ont été collectés.  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/124_Bloc_code_fin.png" alt="fin" width="800"/>

---

# 🎉 3️⃣ Créer la scène de fin

Ouvre la scène **fin**.

## ➕ Ajouter un texte

1️⃣ Ajoute un objet **Texte**  
2️⃣ Écris par exemple *Bravo !* avec une taille de 50px  
3️⃣ Place-le au centre de la scène  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/130_Texte.png" alt="fin" width="800"/>

---

## ➕ Ajouter un bouton "Rejouer"

1️⃣ Ajoute un objet **Bouton** depuis le Magasin de ressources, dans les objets préfabriqués.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/125_Objets_ressource.png" alt="fin" width="800"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/126_Prefabrique.png" alt="fin" width="500"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/128_Boutons.png" alt="fin" width="500"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/129_Bouton.png" alt="fin" width="800"/>

2️⃣ Mets le texte du bouton *Rejouer*
3️⃣ Place-le sous le texte

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/131_Bouton.png" alt="fin" width="800"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/132_Scene.png" alt="fin" width="800"/>

---

# 🔁 4️⃣ Gérer le bouton Rejouer

Dans les **événements de la scène "fin"**, ajoute :

### ➜ Condition

- Le bouton **Rejouer** est cliqué

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/133_Action_bouton.png" alt="fin" width="800"/>

### ➜ Action

- Change de scène → `niveau 1`

👉 Une seule ligne d’événement suffit 🎯

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/134_Code_bouton.png" alt="fin" width="800"/>

---

### Sauvegarder

Pensez à sauvegarder votre projet en cliquant sur la **disquette**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/19_Sauvegarder.png" alt="Évènement" width="400"/>

---  

# ✅ Résultat final

Tu as maintenant :

- 🎮 Un vrai niveau jouable
- 🍗 Des objets à collecter
- 👾 Un ennemi
- ☠️ Une zone de mort
- 🚪 Une porte conditionnelle
- 🏆 Un écran de victoire
- 🔁 Un bouton pour rejouer

🎉 Félicitations !
