# 🎯 Ajuster les masques de collision et tester le jeu

Pour que Dino donne vraiment l’impression de marcher **sur** les plateformes (et pas légèrement dedans ou au-dessus), on va ajuster les **masques de collision**.

---

## 🤔 C’est quoi un masque de collision ?

Le masque de collision définit la **zone réelle de contact** d’un objet.

Même si une image est grande, la zone de collision peut être différente :
- Plus petite
- Plus grande
- Ou mal alignée

👉 Modifier le masque permet d’avoir des collisions propres et réalistes.

---

## 🧱 Modifier le masque de collision d’une plateforme

### Étapes :

1️⃣ Double-clique sur l'objet **Platform_1** (dans la liste des objets à droite)

2️⃣ Clique sur **"Modifier les masques de collision"**  
   (en bas à gauche de la fenêtre)

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/32_Collision.png" alt="Collision" width="600"/>

3️⃣ À droite, clique sur **"Utiliser un masque de collision personnalisé"**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/33_Masque.png" alt="Collision" width="600"/>

4️⃣ Ajuste le masque à gauche en bougeant les points orange :
- Aligne les **deux points orange du haut** exactement au niveau supérieur de la plateforme
- Laisse le masque bien ajusté à la surface sur laquelle Dino doit marcher

*Avant la modification*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/34_Depart.png" alt="Collision" width="600"/>

*Après la modification*  
<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/35_Final.png" alt="Collision" width="600"/>
 
👉 L’objectif est que le haut du masque corresponde parfaitement au sol visible.

5️⃣ Clique sur **"Appliquer"**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/36_Appliquer.png" alt="Collision" width="400"/>

6️⃣ Clique à nouveau sur **"Appliquer"** pour valider les modifications de l’objet

---

## 🔁 Répéter l’opération

Refais exactement la même manipulation pour :

- Platform_2  
- Platform_3  

Toutes les plateformes doivent avoir un masque bien aligné.

---

## ▶️ Lancer l’aperçu

Clique sur **"Aperçu"** (bouton en haut de l’écran).

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/31_Apercu.png" alt="Collision" width="400"/>

🎮 Teste ton jeu :

- ⬅️ ➡️ Flèches directionnelles → déplacer Dino
- ⬆️ ou Barre espace → sauter

---

## ✅ Résultat

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/37_Scene.png" alt="Collision" width="800"/>

- Dino marche proprement sur les plateformes
- Les collisions sont précises
- Le jeu commence à ressembler à un vrai jeu de plateforme 🎉

Prochaine étape : gérer le **déplacement** de notre personnage *Dino* 🔥
