# Firmware

> [!IMPORTANT]
> **À modifier** : décrivez le firmware de votre projet, ou supprimez ce dossier s'il n'y en a pas.

Le **firmware** est le code qui tourne sur la carte électronique (Arduino, ESP32, Raspberry Pi Pico…).
Il se développe avec **VSCode** et l'extension **PlatformIO**
(voir [Installation de VSCode et PlatformIO](https://doc.makerspace-amiens.fr/docs/tutorials/software/vscode-platformio/installation-vscode/)).

- **Carte cible :** …
- **Bibliothèques :** listées dans `platformio.ini` (`lib_deps`), avec leur version

## Organisation

Un dossier par projet PlatformIO :

```text
firmware/
└── mon-robot/
    ├── platformio.ini    carte, framework, bibliothèques
    ├── src/
    │   └── main.cpp      programme principal
    ├── include/          fichiers .h
    └── lib/              bibliothèques écrites par l'équipe
```

Le dossier `.pio/` (fichiers de compilation) est ignoré par git : ne le commitez pas.

## Compiler et téléverser

1. Dans VSCode, ouvrez le dossier du projet PlatformIO (`File > Open Folder` sur
   `firmware/mon-robot/`), pas la racine du repo : sinon PlatformIO ne détecte pas le projet.
2. Branchez la carte en USB.
3. Dans la barre du bas : **✓** pour compiler, **→** pour téléverser, **🔌** pour ouvrir le moniteur série.
<img width="1442" height="932" alt="image" src="https://github.com/user-attachments/assets/f6dc77dd-3dd2-4db5-857e-132023d4b897" />
<img width="1440" height="1920" alt="image" src="https://github.com/user-attachments/assets/960e8bfc-2d23-4cdf-a49f-90ba15fba382" />
<img width="1440" height="1920" alt="image" src="https://github.com/user-attachments/assets/94722ba0-c80d-4be4-a558-22d4dc37f45d" />
