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

**Внимание:** Мы всегда рады новому вкладу в проект. Однако, перед тем, как сделать свой вклад, пожалуйста, прочтите наш [кодекс делового поведения](https://github.com/Grasscutters/Grasscutter/blob/stable/CONTRIBUTING.md).

## Реализованные функции

* Авторизация
* Система боя
* Список друзей
* Телепортация
* Гача-система
* Кооп *работает частично*
* Спавн монстров через консоль
* Функции инвентаря (получение предметов/персонажей, улучшение предметов/персонажей, и т.п.)

## Краткое руководство по установке

**Заметка:** Если вам требуется помощь, присоединитесь к нашему серверу [Discord](https://discord.gg/T5vZU6UyeG) (На Английском).

### Зависимости

* Java SE - 17 ([link](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html))

  **Заметка:** Для того, чтобы просто **запустить сервер**, достаточно только **jre**.

* [MongoDB](https://www.mongodb.com/try/download/community) (рекомендуются версии 4.0+)

* Прокси: mitmdump (рекомендуется), mitmproxy, Fiddler Classic и т.п.

### Запуск

**Заметка:** Для обновления с более старой версии, удалите файл `config.json`, чтобы сгенерировать его заново.

1. Получите файл `grasscutter.jar` одним из следующих способов:
   - Скачайте напрямую со вкладки [Actions](https://github.com/Grasscutters/Grasscutter/suites/6895963598/artifacts/267483297)
   - [Соберите самостоятельно](#Сборка)
2. Создайте папку `resources` в той же директории, что и grasscutter.jar, и переместите туда свои папки `BinOutput` и `ExcelBinOutput` *(Посетите [вики](https://github.com/Grasscutters/Grasscutter/wiki) для получения более подробной информации о том, где их найти.)*
3. Запустите Grasscutter с помощью команды `java -jar grasscutter.jar`. **Убедитесь, что в этот момент запущен сервер mongodb.**

### Соединение с клиентом

½. Создайте аккаунт, введя [соответствующую команду в консоли сервера](https://github.com/Grasscutters/Grasscutter/wiki/Commands#targeting).

1. Перенаправьте трафик: (воспользуйтесь одиним из способов)
    - mitmdump: `mitmdump -s proxy.py -k`

      Доверьтесь сертификату CA:

      ​	**Заметка:** Обычно, сертификат CA хранится в папке `%USERPROFILE%\ .mitmproxy`. Также, вы можете скачать его с `http://mitm.it`

      ​	Дважды нажмите для [установки](https://docs.microsoft.com/ru-ru/skype-sdk/sdn/articles/installing-the-trusted-root-certificate#installing-a-trusted-root-certificate), или же ...

      - С помощью командной строки

        ```shell
        certutil -addstore root %USERPROFILE%\.mitmproxy\mitmproxy-ca-cert.cer
        ```

    - Fiddler Classic: Запустите Fiddler Classic, включите настройку `Decrypt https traffic` в опциях и измените порт по умолчанию (Меню -> Tools -> Options -> Connections) на что-то не равное `8888`, после чего запустите [этот скрипт](https://github.lunatic.moe/fiddlerscript) во вкладке FiddlerSrcipt.

    - [Файл hosts](https://github.com/Grasscutters/Grasscutter/wiki/Running#traffic-route-map)

2. Установите прокси сети в `127.0.0.1:8080`, либо в тот порт прокси, который вы задали.

**Также, вы можете использовать `start.cmd` для автоматического запуска прокси и серверов, но для этого необходимо задать переменную среды JAVA_HOME**

### Сборка

Для сборки и решения проблем с зависимостями, Grasscutter использует Gradle.

**Требуется:**

- [Java SE Development Kits - 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Git](https://git-scm.com/downloads)

##### Windows

```shell
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
.\gradlew.bat # Setting up environments
.\gradlew jar # Compile
```

##### Linux

```bash
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
chmod +x gradlew
./gradlew jar # Compile
```

Получившийся файл .jar можно найти в корневой папке проекта.

### Команды были перемещены на [вики](https://github.com/Grasscutters/Grasscutter/wiki/Commands)!

# Краткое руководство по решению проблем

* Если скомпилировать не удается, то проверьте установку своего JDK (JDK 17 и валидность переменных JDK, bin, PATH)
* Клиент не подключается, не входит, выдаёт ошибку 4206 и т.д. - Скорее всего, проблема в том, *как именно* вы настроили прокси. При использовании
  Fiddler убедитесь, что он запущен на любом порте, кроме 8888
* Порядок запуска: MongoDB > Grasscutter > Прокси (mitmdump, fiddler и т.д.) > Игра
