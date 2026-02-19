# 🔊 Bonus : Ajouter du son dans ton jeu

Un petit son bien placé… et ton jeu prend tout de suite une autre dimension 🎮✨  

On va voir :
- Comment ajouter un son
- Où le déclencher
- Comment éviter qu’il se répète en boucle

---

# 🎵 1️⃣ Ajouter un son

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/135_Ajout_son.png" alt="Bonus" width="800"/>

## Option A — Charger un fichier local

1️⃣ Va dans le gestionnaire des ressources  
2️⃣ Clique sur **Ajouter une ressource**
3️⃣ Sélectionne un fichier audio sur ton ordinateur (`.mp3` ou `.wav`)

👉 Ton son est maintenant disponible dans le projet.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/136_Choix.png" alt="Bonus" width="800"/>

---

## Option B — Créer un son avec JFXR

1️⃣ Ouvre **JFXR** (générateur de sons rétro)
2️⃣ Crée un petit son (ex : saut, pièce collectée, explosion)
3️⃣ Exporte-le en `.wav`
4️⃣ Ajoute-le dans les ressources du projet

👉 Idéal pour des sons style arcade / pixel art 🔥

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/137_Jfxr.png" alt="Bonus" width="800"/>

---

# 🎯 2️⃣ Utiliser le son au bon moment

Le son doit être déclenché **dans le bon événement**.

### Exemple : Son quand Dino ramasse un Chicken Leg

Dans l’événement :

**Condition**
- Collision Dino avec ChickenLeg

**Actions**
- Ajoute 1 à Score
- Supprime ChickenLeg
- ➜ Joue un son (ex: `coin.wav`)

---

# ⚡ 3️⃣ Précharger un son au début de la scène

Pour éviter un petit délai au premier déclenchement :

Ajouter un événement dans la condition **Au lancement de la scène**

### ➜ Action
- Précharger un son

👉 Cela charge le fichier en mémoire dès le départ.

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/139_Precharger.png" alt="Bonus" width="800"/>

---

# 🚨 4️⃣ Éviter que le son se répète en boucle

Si une condition reste vraie plusieurs frames,  
le son peut se rejouer en boucle très vite 😅

### ✅ Solution : Ajouter la condition  
**"Déclencher une seule fois"**

<img src="https://sebastien-devos.fr/img/codegaming/atelier-decouverte/140_Une_fois.png" alt="Bonus" width="800"/>

Exemple :

**Conditions**
- Collision Dino avec Enemy
- Déclencher une seule fois

👉 Le son ne sera joué qu’une seule fois par contact.

---

# 🎮 Où ajouter des sons ?

Quelques idées :

- 🍗 Collecte d’objet
- 🦖 Saut
- 💀 Mort
- 🚪 Porte qui s’ouvre
- 🏆 Victoire

---

# 🎉 Résultat

Avec un son bien placé, ton jeu devient plus vivant et plus dynamique !  
Petit détail… gros impact 🔥
