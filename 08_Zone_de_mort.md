# ☠️ Ajouter une zone de mort

Pour éviter que Dino tombe dans le vide sans conséquence, on va créer une **zone de mort** sous le niveau.

---

## 🎨 Créer l’objet "mort"

1️⃣ Clique sur **Ajouter un nouvel objet**  

2️⃣ Choisis **Nouvel objet à partie de zéro**   

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/79_Nouvel_objet.png" alt="Mort" width="700"/>

3️⃣ Clique sur **Sprite**  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/95_Sprite.png" alt="Mort" width="700"/>

4️⃣ Nomme l’objet : `Mort`  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/96_Mort.png" alt="Mort" width="700"/>

5️⃣ Clique sur **Créer avec Piskel** (éditeur intégré)  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/97_Piskel.png" alt="Mort" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/98_Interface_Piskel.png" alt="Mort" width="700"/>

6️⃣ Crée un bloc de **couleur unie**  en utilisant l'outil *Pot de peinture* et une couleur vive bien visible  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/99_Pot_peinture.png" alt="Mort" width="400"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/100_Couleur_vive.png" alt="Mort" width="400"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/101_Bloc.png" alt="Mort" width="700"/>

7️⃣ Enregistre avec *Save* et ferme Piskel puis **Appliquer**

---

## 📏 Placer la zone de mort

- Glisse l’objet `Mort` dans la scène
- Étire-le pour qu’il couvre **toute la largeur du niveau**
- Place-le **sous les plateformes**, en bas du niveau

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/102_Placement.png" alt="Mort" width="900"/>

👉 Ainsi, si Dino tombe, il touchera cette zone.

💡 Astuce : tu peux réduire son opacité ou le laisser invisible si tu ne veux pas qu’il soit visible en jeu.

---

# 🎬 Ajouter l’événement de mort

Ouvre l’onglet **Événements**.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/38_Onglet_evenements.png" alt="Mort" width="700"/>

## ➕ Créer un nouvel événement

### ➜ Condition
- Dino est en collision avec `Mort`
- Clique à gauche sur ton **Dino**
- Clique au milieu sur **Collision**
- Choisis à droite l'objet **Mort**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/47_Action_Dino.png" alt="Mort" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/72_Collision.png" alt="Mort" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/103_Objet_mort.png" alt="Mort" width="700"/>

### ➜ Actions
- Ajoute une première action : clique à gauche sur **Dino** et au milieu sur **Supprimer** puis Ok  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/77_Supprimer.png" alt="Mort" width="700"/>

- Ajoute une seconde action: dans la recherche à gauche, tape **Attendre** et entre à droite **1 seconde**  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/106_Attendre.png" alt="Mort" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/107_Une_seconde.png" alt="Mort" width="700"/>

- Enfin ajoute une troisième action : changer la scène dans *Autres Actions* puis *Scène* et choisir **Scène sans titre** à droite  

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/104_Changer_scene.png" alt="Mort" width="700"/>

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/105_Scene_sans_titre.png" alt="Mort" width="700"/>

---

# ✅ Résultat

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/108_Code_mort.png" alt="Mort" width="700"/>

- Si Dino tombe dans le vide
- Il touche la zone `mort`
- Le jeu attend 1 seconde
- La scène redémarre

🎉 Ton niveau est maintenant sécurisé ! 

N'oublie pas de **sauvegarder** !

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/19_Sauvegarder.png" alt="Mort" width="400"/>


