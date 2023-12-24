![Grasscutter](https://socialify.git.ci/woailulu/GenshinImpact-PrivateService/image?description=1&descriptionEditable=Liver%20is%20replaced%20by%20deer%0A%2F%2F%5C%5CGenshin%20Impact%20Private%20Service&font=Rokkitt&language=1&logo=https%3A%2F%2Fs2.loli.net%2F2023%2F10%2F29%2F2S7PfkaxUmvqeRo.jpg&name=1&owner=1&pattern=Formal%20Invitation&theme=Dark)


[简中](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/README.md) |
[繁中](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_zh-TW.md) | 
[FR](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_fr-FR.md) | 
[ES](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_es-ES.md) | 
[HE](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_HE.md) |
[RU](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_ru-RU.md) | 
[PL](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_pl-PL.md) | 
[ID](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_id-ID.md) | 
[KR](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_ko-KR.md) | 
[FIL/PH](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_fil-PH.md) | 
[NL](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_NL.md) | 
[JP](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_ja-JP.md) | 
[IT](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_it-IT.md) | 
[VI](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_vi-VN.md) | 
[हिंदी](https://github.com/woailulu/GenshinImpact-PrivateService/blob/%E9%87%8D%E7%82%B9/%E7%95%8C%E9%9D%A2/README_hn-IN.md)

**Attention:** De nouveaux contributeurs sont toujours les bienvenus. Avant d'ajouter votre contribution, veuillez lire le [code de conduite](https://github.com/Grasscutters/Grasscutter/blob/stable/CONTRIBUTING.md).

## Fonctionnalités actuelles :

* Connection
* Combat
* Liste d'amis
* Téléportation
* Système de gacha
* Le multijoueur fonctionne *partiellement*
* Apparition de monstres via la console
* Inventaire (obtention d'objets/de personnages, amélioration d'objets/personnages, etc)

## Guide d'installation rapide

**Note:** Pour obtenir un support, rejoignez notre serveur [Discord](https://discord.gg/T5vZU6UyeG) (en anglais).

### Démarage rapide (Automatique)

- Téléchargez Java 17: https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html
- Téléchargez [MongoDB Community Server](https://www.mongodb.com/try/download/community)
- Téléchargez la version du jeu REL3.7 (Le client de jeut peut être obtenu ici si vous ne l'avez pas): https://github.com/MAnggiarMustofa/GI-Download-Library/blob/main/GenshinImpact/Client/3.7.0.md

- Téléchargez la [dernière version de Cultivation](https://github.com/Grasscutters/Cultivation/releases/latest). Ulilisez l'installateur en `.msi`.
- Après avoir ouvert Cultivation (en administrateur), appuyez sur le bouton de téléchargement en haut a droite. 
- Cliquez sur le bouton `Téléchargez tout-en-un`
- Cliquez sur l'engrenage dans le coin en haut a droite.
- Définisez l'emplacement d'installation du jeu.
- Définisez le chemin Java personnalisé à `C:\Program Files\Java\jdk-17\bin\java.exe`
- Laissez tous les autres paramètes par défauts

- Appuyez sur le bouton a coté de Lancer.
- Appuyez sur le bouton Lancer.
- Connectez vous avec le nom d'utilisateur que vous voulez. Le mot de passe n'a pas d'importance.

### Compilation

Grasscutter utilise Gradle pour la gestion des dépendances et la compilation.

**Prérequis**

- [Java SE Development Kits - 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html) ou plus récent
- [Git](https://git-scm.com/downloads)

##### Windows

```shell
git clone --recurse-submodules https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
.\gradlew.bat # Setting up environments
.\gradlew jar # Compile
```

##### Linux (GNU)

```bash
git clone --recurse-submodules https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
chmod +x gradlew
./gradlew jar # Compile
```

Vous pouvez trouver le jar de sortie dans la racine du dossier du projet.

### Dépanage

Pour une liste des problèmes communs et leur solution et pour demander de l'aide, veuillez rejoindre [notre serveur Discord](https://discord.gg/T5vZU6UyeG) (en anglais) et dirigez vous vers le salon de support.
