# ESP32-BLE-FruitBuster

> ### 🚫 Warning
> Only use this on devices you own or when you have permisson to use it.\
> This project is made for educational purposes ONLY and is NOT made to break laws and/or\
> for personal gain. Everythin is provided as-is and has no warranty so if your break any of your devices.

![ESP32 BLE](https://img.shields.io/badge/ESP32-BLE-blue.svg) ![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-green.svg)

Un projet fun et éducatif pour ESP32 exploitant le BLE pour envoyer des notification de connexion d'appareils sur les appareils Apple ! Il permet de simuler des AirPods, une Apple TV ect... ou d’envoyer des paquets Apple pour faire planter les iOS 17. **À utiliser avec responsabilité !**

## 🚀 Fonctionnalités
- **🔹 Mode Simulation** : Se fait passer pour un appareil Apple (AirPods, Apple TV, etc.).
- **⚠️ Mode Sour Apple** : Envoie des paquets BLE pour perturber les dispositifs iOS à proximité.
- **💡 LED Feedback** :
  - Fixe en mode Simulation.
  - Clignotante en mode Sour Apple.
- **🎛️ Contrôle via le bouton BOOT (GPIO 0)** pour changer de mode.

## 🛠️ Installation
1. **Cloner le dépôt** :
   ```bash
   git clone https://github.com/xClem123/ESP32-BLE-FruitBuster.git
   ```
2. Ouvrir dans l'IDE Arduino.
  - Installer les dépendances :
  - Bibliothèque BLE (ESP32 standard).
  - Bibliothèque NimBLE-Arduino (via le gestionnaire de bibliothèques).
    
3. Téléverser le code sur l’ESP32.
 
## 🎮 Utilisation
- Mode 0 : Désactivé (LED éteinte).
- Mode 1 : Simulation Apple (LED fixe).
- Mode 2 : Attaque Sour Apple (LED clignote).
- Changer de mode : Appuyer sur BOOT (GPIO 0).
  
## ⚠️ Changelog
- **2025-03-10**
- Correction Bug Compilation : Résolution des conflits entre BLEDevice.h et NimBLEDevice.h. Passage exclusif à NimBLEDevice.h pour les deux modes (Simulation Apple et Sour Apple). Correction des appels à addData et suppression des méthodes incompatibles - (setAdvertisementType, setDeviceAddress).


## 📜 Crédits
- [RapierXbox](https://github.com/RapierXbox/ESP32-Sour-Apple) : Pour le code Sour Apple.
- [ckcr4lyf](https://github.com/ckcr4lyf/EvilAppleJuice-ESP32) : Base de code pour le BLE spam.
  
## 📜 Licence
Ce projet est sous licence GNU GPL v3.0. Voir le fichier LICENSE pour plus de détails.
