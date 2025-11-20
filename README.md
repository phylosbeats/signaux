# 🧠 Application de singaux aléatoires

Une application web minimaliste, contenue dans un seul fichier HTML, conçue pour envoyer des signaux lumineux et/ou sonores aléatoirement.

L'utilisateur est face à un écran noir pendant une durée déterminée (2 minutes). Des stimuli aléatoires (visuels et/ou auditifs) apparaissent à des intervalles imprévisibles (fixés entre 2 et 7 secondes d'intervalle).

## 📋 Fonctionnalités

* **Atmosphère immersive :** Interface totalement noire pour limiter les distractions.
* **Stimuli aléatoires :**
    * 👁️ **Visuel :** L'écran clignote (flash stroboscopique 2 fois).
    * 🔊 **Auditif :** Un bip sonore (généré via Web Audio API).
    * 🔀 **Mixte :** Apparition simultanée du flash et du bip.
* **Logique imprévisible :** Les signaux apparaissent à des moments aléatoires (intervalles variables).
* **Timer discret :** Un compte à rebours est affiché en bas de page en gris foncé pour ne pas attirer l'œil inutilement.
* **Zéro dépendance :** Pas d'images, pas de fichiers MP3 externes, pas de frameworks. Tout est généré par le code.

## 🚀 Comment l'utiliser

Aucune installation n'est nécessaire.

1.  Téléchargez ou clonez ce dépôt.
2.  Ouvrez le fichier `index.html` dans votre navigateur web (Chrome, Firefox, Edge, Safari).
3.  Cliquez sur le bouton **LANCER** pour démarrer la session (ce clic est nécessaire pour autoriser le navigateur à jouer du son).

## 🛠️ Configuration / Personnalisation

Vous pouvez facilement modifier les paramètres en éditant le script dans le fichier `index.html`.

### Changer la durée
Cherchez la variable `DURATION` (ligne ~80) :
```javascript
const DURATION = 120; // Durée en secondes (ici 2 minutes)