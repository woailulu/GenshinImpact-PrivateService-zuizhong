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


**＊:** 私たちはプロジェクトへの貢献者をいつでも歓迎します。貢献を追加する前に、我々の [行動規範](https://github.com/Grasscutters/Grasscutter/blob/stable/CONTRIBUTING.md)をよくお読みください。

## 現在機能している物

* ログイン
* 戦闘
* フレンドリスト
* テレポート
* 祈願(ガチャ)
* マルチプレイは一部機能しています
* コンソールを使用してモンスターをスポーンさせる
* インベントリ機能 (アイテム/キャラクターの受け取り､アイテム/キャラクターのアップグレードなど)

## クイックセットアップガイド

**＊:** サポートが必要な場合はGrasscutterの[Discord](https://discord.gg/T5vZU6UyeG)に参加してください。

### 動作環境

* [JAVAのバージョン17以降](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)

  **＊:** サーバーを動作させるだけならjreのみで十分です｡ 開発をしたい場合JDKが必要になるかもしれません。

* [MongoDB](https://www.mongodb.com/try/download/community) (バージョン4.0以降を推奨)

* プロキシツール: [mitmproxy](https://mitmproxy.org/) (mitmdump, 推奨)、[Fiddler Classic](https://telerik-fiddler.s3.amazonaws.com/fiddler/FiddlerSetup.exe)、その他｡

### 起動方法

**＊:** もしサーバーをアップデートしたい場合は`config.json`を削除してから再生成してください。

1. `grasscutter.jar`を入手する
   - [releases](https://github.com/Grasscutters/Grasscutter/releases/latest) か [action](https://github.com/Grasscutters/Grasscutter/actions) からダウンロードするか、[自分でビルド](#ビルド)してください｡
2. `grasscutter.jar` があるディレクトリに `resources` フォルダーを作成し、そこに `BinOutput, ExcelBinOutput, Readables, Scripts, Subtitle, TextMap` を移動してください *(`resources` フォルダの中身の入手方法については [wiki](https://github.com/Grasscutters/Grasscutter/wiki) を参照してください.)*
3. コマンドプロンプトに`java -jar grasscutter.jar`を入力しGrasscutterを起動してください。**このときMongoDBも実行する必要があります。**

### クライアントとの接続

½. [このコマンド](https://github.com/Grasscutters/Grasscutter/wiki/Commands#commands-for-server-admins)をサーバーコンソールから使用してアカウントを作成してください｡

1. 通信内容をリダイレクトする: (どちらか一つを選択してください)
    - mitmdump: `mitmdump -s proxy.py -k`

      - CA証明書を信頼する:

        - **＊:** CA証明書は`%USERPROFILE%\.mitmproxy`に保存されています。ダブルクリックして[インストール](https://docs.microsoft.com/en-us/skype-sdk/sdn/articles/installing-the-trusted-root-certificate#installing-a-trusted-root-certificate)するか...

        - コマンドライン経由でインストールします

        ```shell
        certutil -addstore root %USERPROFILE%\.mitmproxy\mitmproxy-ca-cert.cer
        ```

    - Fiddler Classic: Fiddler Classicを起動し(Tools -> Options -> HTTPS)から`Decrypt https traffic`をオンにしてください｡ (Tools -> Options -> Connections) に有るポート番号の設定を`8888`以外に設定してください。その後この[スクリプト](https://github.com/Grasscutters/Grasscutter/wiki/Resources#fiddler-classic-jscript)をFiddlerScriptタブにコピペしてロードします。

    - [ホストファイル](https://github.com/Grasscutters/Grasscutter/wiki/Resources#hosts-file)

2. ネットワークプロキシを `127.0.0.1:(自分で設定したポート番号)` に設定してください｡
- mitmproxyを使用した場合：プロキシの設定と証明書のインストールが終わった後、http://mitm.it/ でトラフィックがmitmproxyを通過しているか確認しましょう。

**`start.cmd`でmitmdumpとサーバーをまとめて起動することが出来ます。ただ、事前に`start_config.cmd`でJAVAのパスを指定している必要があります。**

### ビルド

GrasscutterはGradleを使用して依存関係とビルドを処理しています。

**要件:**

- [Java SE Development Kits - 17以降](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Git](https://git-scm.com/downloads)

##### Windows

```shell
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
.\gradlew.bat # コンパイル環境の構築
.\gradlew jar # コンパイル
```

##### Linux

```bash
git clone https://github.com/Grasscutters/Grasscutter.git
cd Grasscutter
chmod +x gradlew
./gradlew jar # コンパイル
```

生成されたjarファイルはプロジェクトフォルダのルートに有ります。

### コマンドリストは[wiki](https://github.com/Grasscutters/Grasscutter/wiki/Commands)へ移動しました｡

# トラブルシューティング

* コンパイルが失敗した場合JDKがインストールされているか確認してください。(JDKのバージョンが17以降であることと、環境変数でJDKのパスが設定されている必要があります)
* クライアントが接続できない・ログインできない・エラーコード4206・またその他場合、ほとんどは、プロキシデーモンの設定が問題です。Fiddlerを使っている場合はデフォルトポートを8888以外の別のポートに変更してみてください。
  Fiddlerを使用している場合はポートが8888以外に設定されていることを確認してください。
* 起動シーケンス(順番): MongoDB > Grasscutter > プロキシツール (mitmdumpかfiddler、その他) > ゲーム
