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

**Perhatian:** Kami selalu menyambut kontributor untuk proyek ini. Sebelum menambahkan kontribusi Anda, harap baca [Kode Etik](https://github.com/Grasscutters/Grasscutter/blob/stable/CONTRIBUTING.md) kami.

## Fitur terkini

* Logging in
* Pertempuran
* Daftar teman
* Teleportasi
* Sistem gacha
* Co-op *sebagian* berfungsi
* Memunculkan monster melalui konsol
* Fitur inventaris (menerima item/karakter, meng-upgrade item/karakter, dll)

## Panduan penyiapan cepat

**Catatan:** Untuk dukungan, silakan bergabung dengan [Discord](https://discord.gg/T5vZU6UyeG) kami.

### Requirements

* Java SE - 17 ([link](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html))

  **Catatan:** Jika Anda hanya ingin **menjalankannya**, maka **jre** saja sudah cukup.

* [MongoDB](https://www.mongodb.com/try/download/community) (recommended 4.0+)

* Daemon proksi: mitmproxy (mitmdump, direkomendasikan), Fiddler Classic, etc.

### Menjalankan

**Catatan:** Jika Anda memperbarui dari versi lama, hapus `config.json` untuk membuatnya kembali.

1. Dapatkan `grasscutter.jar`
   - Download dari [actions](https://github.com/Grasscutters/Grasscutter/suites/6895963598/artifacts/267483297)
   - [Bangun sendiri](#Membangun)
2. Buat folder `resources` di direktori tempat grasscutter.jar berada dan pindahkan folder `BinOutput` dan `ExcelBinOutput` ke sana *(Periksa [wiki](https://github.com/Grasscutters/Grasscutter/wiki) untuk detail lebih lanjut tentang cara mendapatkannya.)*
3. Jalankan Grasscutter dengan `java -jar grasscutter.jar`. **Pastikan layanan mongodb juga berjalan.**

### Connecting to the client

½. Buat akun dengan menggunakan [server console command](https://github.com/Grasscutters/Grasscutter/wiki/Commands#targeting).

1. Pengalihan traffic: (pilih salah satu)
    - mitmdump: `mitmdump -s proxy.py -k`

      Trust CA certificate:

      ​**Catatan:** Sertifikat CA biasanya disimpan di `%USERPROFILE%\ .mitmproxy`, atau anda dapat download dari  `http://mitm.it`

      ​	klik dua kali untuk [menginstall](https://docs.microsoft.com/en-us/skype-sdk/sdn/articles/installing-the-trusted-root-certificate#installing-a-trusted-root-certificate) ataupun juga

      - melalui command line

        ```shell
        certutil -addstore root %USERPROFILE%\.mitmproxy\mitmproxy-ca-cert.cer
        ```

    - Fiddler Classic: Jalankan Fiddler Classic, nyalakan `Decrypt https traffic` dalam setting dan ubah port default di sana (Tools -> Options -> Connections) ke apa pun selain `8888`, dan muat [skrip ini](https://github.lunatic.moe/fiddlerscript).

    - [File host](https://github.com/Grasscutters/Grasscutter/wiki/Running#traffic-route-map)

2. Atur proxy jaringan ke `127.0.0.1:8080` atau port proxy yang anda tentukan.

**Anda juga dapat menggunakan `start.cmd` untuk memulai server dan proxy daemon secara otomatis, tetapi Anda harus mengatur JAVA_HOME enviroment**

### Membangun

Grasscutter menggunakan Gradle untuk menangani dependensi & pembangunan.

**Requirements:**

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

Anda bisa menemukan output jar di root folder proyek.

### Commands telah dipindahkan ke [wiki](https://github.com/Grasscutters/Grasscutter/wiki/Commands)!

# Quick Troubleshooting

* Jika kompilasi tidak berhasil, periksa instalasi JDK Anda (JDK 17 dan validasi variabel bin PATH JDK)
* Klien saya tidak terhubung, tidak login, 4206, dan lain-lain - Sebagian besar pengaturan daemon proxy Anda adalah *masalahnya*, jika menggunakan
Fiddler pastikan berjalan pada port lain kecuali 8888
* Urutan startup: MongoDB > Grasscutter > Proxy daemon (mitmdump, fiddler, etc.) > Game
