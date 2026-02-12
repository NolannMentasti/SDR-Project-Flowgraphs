# 📡 SDR Project: Reverse Engineering & Jamming (27 MHz)

Ce dépôt contient les ressources techniques de mon projet académique sur la **Radio Logicielle (SDR)**.
L'objectif était de rétro-ingénierier un char radio-commandé, d'analyser son protocole et de tester des vulnérabilités physiques.

🔗 **Voir le portfolio complet :** www.nolann-mentasti.fr

## 🛠️ Stack Technique
* **Matériel :** HackRF One, Antennes télescopiques
* **Logiciel :** GNU Radio Companion, Python
* **Cible :** Char RC (Fréquence 27 MHz, Modulation OOK)

## 📂 Contenu du dépôt

### 1. Analyse & Décodage (`/flowgraphs`)
* `analysis_fft.grc` : Visualisation du spectre et isolation de la porteuse.
* `demodulation_ook.grc` : Chaîne de traitement pour démoduler le signal On-Off Keying.

### 2. Attaques (`/flowgraphs`)
* **Replay Attack :** Capture d'une trame valide ("Avancer") et réémission brute pour contrôler le véhicule.
* **Jamming (Brouillage) :**
    * *Smart Jamming :* Génération de bruit blanc ciblé sur 27.145 MHz.
    * *Mass Jamming :* Saturation large bande (moins efficace).

## 🚀 Comment utiliser
1.  Installer **GNU Radio** (v3.10+ recommandé).
2.  Cloner ce dépôt.
3.  Ouvrir un fichier `.grc` dans GNU Radio Companion.
4.  Brancher le HackRF One.
5.  Exécuter le flowgraph.

## ⚠️ Avertissement
Ce projet a été réalisé dans un cadre éducatif strict, sur du matériel appartenant à l'IUT, dans une zone contrôlée (Cage de Faraday ou faible puissance). L'émission radio est réglementée.

---
*Auteur : Nolann Mentasti*
