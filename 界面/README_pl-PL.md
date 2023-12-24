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


**Uwaga:** Zawsze jesteśmy otwarci na wasz wkład w projekt. Przed zaproponowaniem zmian przeczytaj [zasady postępowania (ENG)](https://github.com/Grasscutters/Grasscutter/blob/stable/CONTRIBUTING.md).

## Obecne funkcje

* Logowanie się
* Walka
* Lista przyjaciół
* Teleportacja
* System losowania
* *Częściowo* działający co-op
* Wzywanie potworów przez konsolę
* Działający ekwipunek (otrzymywanie przedmiotów/postaci, ulepszanie przedmiotów/postaci, itp)

## Poradnik uruchamiania

**Uwaga:** Dla dodatkowej pomocy dołącz na nasz [Discord](https://discord.gg/T5vZU6UyeG).

### Wymagania

* Java SE - 17 ([link](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html))

  **Uwaga:** Jeśli chcesz tylko **uruchomić** serwer, samo **jre** powinno wystarczyć.

* [MongoDB](https://www.mongodb.com/try/download/community) (rekomendowane 4.0+)

* Aplikacja proxy: mitmproxy (mitmdump, rekomendowane), Fiddler Classic, itp.

### Uruchamianie

**Uwaga:** Jeśli aktualizujesz ze starszej wersji, usuń `config.json` aby wygenerować go ponownie.

1. Zdobądź `grasscutter.jar`
   - Pobierz z [akcji](https://github.com/Grasscutters/Grasscutter/suites/6895963598/artifacts/267483297)
   - [Lub zbuduj to samemu](#Budowanie)
2. Utwórz folder `resources` w tym samym folderze gdzie znajduje się grasscutter.jar oraz przenieś foldery `BinOutput` i `ExcelBinOutput` do folderu `resources` *(Sprawdź na [wiki](https://github.com/Grasscutters/Grasscutter/wiki) skąd możesz je pozyskać).*
3. Uruchom Grasscuttera komendą `java -jar grasscutter.jar`. **Upewnij się, że mongodb service działa w tle.**

### Łączenie się z klientem

½. Utwórz konto za pomocą [komend konsoli serwera](https://github.com/Grasscutters/Grasscutter/wiki/Commands#targeting).

1. Przekieruj połączenia: (wybierz jedno)
    - mitmdump: `mitmdump -s proxy.py -k`

      Certyfikat CA:

      ​	**Uwaga:** CA certyfikat zazwyczaj znajduje się w `%USERPROFILE%\.mitmproxy`, albo możesz pobrać go stąd `http://mitm.it`

      ​	Naciśnij podwójnie, aby [zainstalować](https://docs.microsoft.com/en-us/skype-sdk/sdn/articles/installing-the-trusted-root-certificate#installing-a-trusted-root-certificate) lub ...

      - Za pomocą wierszu poleceń (lub PowerShella) wpisz

        ```shell
        certutil -addstore root %USERPROFILE%\.mitmproxy\mitmproxy-ca-cert.cer
        ```

    - Fiddler Classic: Uruchom Fiddler Classic, włącz `Decrypt https traffic` w ustawieniach oraz zmień domyślny port (Tools -> Options -> Connections) na dowolny inny niż `8888`, i wczytaj [ten skrypt](https://github.lunatic.moe/fiddlerscript) (w polu FiddlerScript).

    - [Plik hosts](https://github.com/Grasscutters/Grasscutter/wiki/Running#traffic-route-map)

2. Ustaw serwer proxy na `127.0.0.1:8080` albo inny wybrany przez ciebie port.

**Możesz także użyć `start.cmd` aby uruchomić serwer gry i proxy, ale do tego musisz ustawić środowisko JAVA_HOME**

### Budowanie

Grasscutter używa Gradle, aby zajął się wymaganymi pakietami i kompilowaniem.

**Wymagania:**

- [Java SE Development Kits - 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Git](https://git-scm.com/downloads)

##### Windows

```shell
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
.\gradlew.bat # Konfigurowanie środowiska
.\gradlew jar # Kompilowanie
```

##### Linux

```bash
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
chmod +x gradlew
./gradlew jar # Kompilowanie
```

Gotowy plik `jar` możesz znaleźć w głównym folderze Grasscuttera.

### Komendy zostały przeniesione do [wiki](https://github.com/Grasscutters/Grasscutter/wiki/Commands)!

# Rozwiązywanie problemów

* Jeśli kompilowanie się nie powiodło, sprawdź swoje zainstalowane JDK (JDK 17 oraz wartość ścieżki (PATH) folderu bin należącego do JDK)
* Mój klient nie może się połączyć, nie działa logowanie, 4206, itp... - Prawdopodobnie twoje proxy jest *problemem*, jeśli używasz Fiddlera upewnij się, że działa na innym porcie niż 8888
* Sekwencja, którą powinieneś uruchamiać: MongoDB > Grasscutter > Proxy daemon (mitmdump, fiddler, etc.) > Game
