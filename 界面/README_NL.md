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

**Aantekening:** We verwelkomen altijd bijdragers aan het project. Lees onze [Gedragscode](https://github.com/Grasscutters/Grasscutter/blob/development/README_NL.md#bijdragen-aan-het-project) zorgvuldig door voordat u uw bijdrage toevoegt.

## Huidige functies

* inloggen
* Combat
* Vriendenlijst
* Teleportatie
* Gacha systeem
* Co-op werkt (gedeeltelijk)
* Monsters spawnen via console
* Inventaris functies (ontvangen van items / karakters, upgraden van items / karakters, enz.)


## Snelle installatie gids

**Note:** Voor ondersteuning kunt u lid worden van onze [Discord](https://discord.gg/T5vZU6UyeG).

### Vereisten

* [Java SE - 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)

  **Note:** Als u het alleen wilt **draaien**, dan is **jre** alleen prima.

* [MongoDB](https://www.mongodb.com/try/download/community) (aanbevolen 4.0+)

* Proxy Daemon: [mitmproxy](https://mitmproxy.org/) (mitmdump, aanbevolen), [Fiddler Classic](https://telerik-fiddler.s3.amazonaws.com/fiddler/FiddlerSetup.exe), enz.

### Opstarten

**Note:** Als u vanaf een oudere versie heeft geupdate, verwijder dan `config.json` om het te regenereren.

1. Verkrijg `grasscutter.jar`
   - Download van [actions](https://github.com/Grasscutters/Grasscutter/actions) of [bouw de jar zelf](#Bouwen)
2. Maak een `resources` map aan in de directory waar grasscutter.jar staat en verplaats je `BinOutput, ExcelBinOutput, Readables, Scripts, Subtitle, TextMap` mappen daarheen *(Check de [wiki](https://github.com/Grasscutters/Grasscutter/wiki) voor meer details hoe je die krijgt.)*
3. Start Grasscutter met `java -jar grasscutter.jar`. **Zorg ervoor dat de mongodb service ook draait.**

### Verbinden met de client

½. Maak een account aan met [server console command](https://github.com/Grasscutters/Grasscutter/wiki/Commands#targeting).

1. Verkeer omleiden: (kies er een)
    - mitmdump: `mitmdump -s proxy.py -k`

      Vertrouw CA certificaat:

      **Note:** Het CA certificaat is meestal opgeslagen in `%USERPROFILE%.mitmproxy`, of je kan het downloaden van `http://mitm.it`

      Dubbelklik voor [install](https://docs.microsoft.com/en-us/skype-sdk/sdn/articles/installing-the-trusted-root-certificate#installing-a-trusted-root-certificate) of ...

      - Via de commandoregel

        ```Shell
        certutil -addstore root %USERPROFILE%%%.mitmproxymitmproxy-ca-cert.cer
        ```

    - Fiddler Classic: Start Fiddler Classic, zet `Decrypt https traffic` aan in setting en verander de standaard poort daar (Tools -> Options -> Connections) in iets anders dan `8888`, en laad [dit script](https://github.com/Grasscutters/Grasscutter/wiki/Resources#fiddler-classic-jscript).

    - [Hosts file](https://github.com/Grasscutters/Grasscutter/wiki/Resources#hosts-file)

2. Stel de netwerk proxy in op `127.0.0.1:8080` of de proxy poort die u heeft opgegeven.

**U kunt ook `start.cmd` gebruiken om servers en proxy daemons automatisch te starten, maar dan moet u JAVA_HOME enviroment en `start_config.cmd` instellen.**

### Bouwen

Grasscutter gebruikt Gradle om afhankelijkheden en bouwen af te handelen.

**Vereisten:**

- [Java SE Development Kits - 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Git](https://git-scm.com/downloads)

##### Windows

```Shell
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
.\gradlew.bat # Instellen van omgevingen
.gradlew jar # Compileren
```

##### Linux

```bash
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
chmod +x gradlew
./gradlew jar # Compileer
```

U kunt de output jar vinden in de root van de project map.

### Commando's zijn verplaatst naar de [wiki](https://github.com/Grasscutters/Grasscutter/wiki/Commands)!

# Quick Troubleshooting

* Als het compileren niet succesvol was, controleer dan je JDK installatie (JDK 17 en gevalideerde JDK's bin PATH variabele)
* Mijn client maakt geen verbinding, logt niet in, 4206, etc... - Meestal is je proxy daemon setup *het probleem*, als je
  Fiddler gebruik, zorg ervoor dat het op een andere poort draait behalve 8888
* Opstart volgorde: MongoDB > Grasscutter > Proxy daemon (mitmdump, fiddler, enz.) > Game




# Bijdragen aan het project

Let op: we hebben een gedragscode, volg deze alsjeblieft in al je interacties met het project. Als je nog vragen hebt, maak dan een issue aan of vraag het in de Discord server.

- Repareer/toevoeg alleen de functionaliteit in kwestie OF pak wijdverspreide witruimte/stijl problemen aan, niet beide.
- Pak een enkel probleem aan met zo min mogelijk gewijzigde regels.

**Maak geen pull request om samen te voegen in stable tenzij het een hotfix is. Gebruik in plaats daarvan de development branch.**

## Pull Request Proces

1. Zorg ervoor dat alle installatie- of build-afhankelijkheden verwijderd zijn voor het einde van de laag wanneer u een build doet.
2. 2. Werk de README.md en wiki bij met details van wijzigingen aan de interface, inclusief nieuwe omgevingsvariabelen, blootgestelde poorten, nuttige bestandslocaties en containerparameters.
3. Schrijf met detail op je pull request beschrijving wat je hebt gecommit, om het makkelijker te maken voor de medewerkers om een changelog te maken.
