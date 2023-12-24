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


**Atención:** Siempre damos la bienvenida a contribuidores del proyecto. Antes de añadir tu contribución, por favor lee cuidadosamente nuestro [Código de conducta](https://github.com/Grasscutters/Grasscutter/blob/stable/CONTRIBUTING.md).

## Funcionalidades actuales

* Iniciar sesión
* Combate
* Lista de amigos
* Teletransportación
* Sistema Gacha
* Cooperativo *parcialmente* funcional
* Invocar monstruos desde la consola
* Funcionalidades de inventario (recibir objetos/personajes, mejorar objetos/personajes, etc)

## Guía rápida de configuración

**Nota:** Para soporte, únete a nuestro [Discord](https://discord.gg/T5vZU6UyeG).

### Requerimientos

* Java SE - 17 ([link](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html))

  **Nota:** Si solo quieres **ejecutarlo**, entonces **jre** es suficiente.

* [MongoDB](https://www.mongodb.com/try/download/community) (recomendado 4.0+)

* Servicio de proxy: mitmproxy (mitmdump, recomendado), Fiddler Classic, etc.

### Ejecución

**Nota:** Si actualizaste de una versión anterior, elimina `config.json` para que se genere de nuevo.

1. Consigue `grasscutter.jar`
   - Descarga desde [actions](https://github.com/Grasscutters/Grasscutter/suites/6895963598/artifacts/267483297)
   - [Constrúyelo tu mismo](#Construcción)
2. Crea una carpeta `resources` en el directorio donde se encuentra grasscutter.jar y mueve las carpetas `BinOutput` y `ExcelBinOutput` ahí *(Consulta la [wiki](https://github.com/Grasscutters/Grasscutter/wiki) para más detalles de como conseguirlos.)*
3. Ejecuta Grasscutter con `java -jar grasscutter.jar`. **Asegúrate de que el servicio de mongodb está activo.**

### Conexión con el cliente

½. Crea una cuenta usando [el comando correspondiente en la consola del servidor](https://github.com/Grasscutters/Grasscutter/wiki/Commands#targeting).

1. Redirecciona el tráfico: (elegir uno)
    - mitmdump: `mitmdump -s proxy.py -k`

      Autoriza el certificado CA:

      ​	**Nota:**El certificado CA normalmente se encuentra en `%USERPROFILE%\ .mitmproxy`, o puedes descargarlo de `http://mitm.it`

      ​	Doble clic para [instalar](https://docs.microsoft.com/en-us/skype-sdk/sdn/articles/installing-the-trusted-root-certificate#installing-a-trusted-root-certificate) o ...

      - Con línea de comandos

        ```shell
        certutil -addstore root %USERPROFILE%\.mitmproxy\mitmproxy-ca-cert.cer
        ```

    - Fiddler Classic: Ejecuta Fiddler Classic, activa `Decrypt https traffic` en las opciones y cambia el puerto por defecto ahí (Herramientas -> Opciones -> Conexiones) a alguno que no sea `8888`, y carga [este script](https://github.lunatic.moe/fiddlerscript).

    - [Archivo Hosts](https://github.com/Grasscutters/Grasscutter/wiki/Running#traffic-route-map)

2. Establece el proxy de red a `127.0.0.1:8080` o el puerto de proxy que pusiste.

**También puedes usar `start.cmd` para iniciar el servidor y el servicio de proxy automáticamente, pero tienes que configurar el entorno JAVA_HOME**

### Construcción

Grasscutter usa Gradle para manejar dependencias y construcción.

**Requerimientos:**

- [Java SE Development Kits - 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Git](https://git-scm.com/downloads)

##### Windows

```shell
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
.\gradlew.bat # Configuración de entornos
.\gradlew jar # Compilar
```

##### Linux

```bash
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
chmod +x gradlew
./gradlew jar # Compilar
```

Podrás encontrar el jar generado en la carpeta raíz del proyecto.

### ¡Los comandos han sido movidos a la [wiki](https://github.com/Grasscutters/Grasscutter/wiki/Commands)!

# Soluciones a errores comunes

* Si la compilación falla, por favor comprueba tu instalación de JDK (JDK 17 y valida la variable bin PATH del JDK)
* Mi cliente no conecta, no inicia sesión, 4206, etc... - Probablemente, tu configuración del proxy es *el problema*, si usas
  Fiddler asegúrate de que está usando un puerto distinto al 8888
* Secuencia de inicio: MongoDB > Grasscutter > Servicio de proxy (mitmdump, fiddler, etc.) > Juego
