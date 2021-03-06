
# 4. トラブルシューティング

[English](./en_troubleshooting.html)

## 4.1. キャラクター付近のコントロールパネルや他のアプリケーションがクリックに反応しない

v0.8.2aまたはそれ以前のバージョンでこの問題が起こる事があります。

キャラクター付近をクリックしたままドラッグしてキャラクターが移動するか確認します。

もし移動出来る場合は、離れた位置にキャラクターを退避し、再度試してみてください。

何度もキャラクターを動かすのが面倒な場合、キャラクターを移動後にコントロールパネルの`配信`タブで、`(背景透明時)キャラ付近を掴んでドラッグ移動`のチェックをオフにします。

詳しくは[2: 基本的な使い方](./get_started.html)の"2.3.1. ウィンドウ"をご確認下さい。


## 4.2. 起動直後にVMagicMirrorが停止する

設定ファイルが破損している可能性があり、設定の初期化が必要です。

この場合、次の手順を順に試します。

* コントロールパネルの`ホーム`タブで、右側にある`リセット`ボタンを押します。確認ダイアログが出るので`OK`を押して設定をリセットします。
    + これで復帰したように見える場合、[2: 基本的な使い方](./get_started.html)の手順でセットアップします。
* 上記の方法で直らない場合、いったんVMagicMirrorを終了します。
* `VMagicMirror.exe`があるフォルダ以下の`ConfigApp`フォルダを開き、`_autosave`という名前のファイルを削除します。その後、`VMagicMirror`を再び起動します。


## 4.3. CPU負荷が高すぎる

コントロールパネルの`配信`タブで、リップシンクや顔トラッキングを無効化します。

ゲームパッドを使わない場合、

* コントロールパネルの`ホーム`タブで`設定ウィンドウを開く`ボタンを押して設定ウィンドウを開きます。
* `レイアウト`タブの`ゲームパッド`を参照し`ゲームパッド入力のキャプチャを有効化`のチェックをオフにします。


## 4.4. 視線トラッキングがうまく動かない

プレイしているソフトによっては仕様(※下部参照)となります。ご了承ください。

場合によっては見栄えが改善するカスタマイズとして、マウス追尾を無効化し、代わりに常に正面を見るようにした方が自然になるかもしれません。

* コントロールパネルの`配信`タブで`顔・表情`メニュー下の`視線の動き`を`固定`に変更します。


※以下はこのトラブルの発生原因です。

一部のFPS等のゲームでは、ゲームの実行中つねにマウスをウィンドウ中央に寄せるプログラムが動作します。

このため物理的にマウスを動かしてもポインター位置が変わらず、キャラクターの首が動かない、という挙動になります。

有名なソフトでこの挙動がおきる例として、VRChatのデスクトップモードなどが該当します。



## 4.5. まばたきをトラッキングしない

メガネをかけている場合、外して試してみてください。

メガネをかけていると表情認識に失敗して「つねに目を見開いている」と判定してしまう事があります。

もしそうでない場合、カメラが顔全体の表情をはっきりと捉えられるよう、以下のことを確認してください。

* カメラから丁度よい距離にいること
* 髪が顔にかかりすぎていないこと
* 部屋がじゅうぶん明るいこと
* 首元がすっきりした服を着ていること
* 口元が隠れすぎていないこと (マイクで一部が隠れる程度はOKです)

## 4.6. キャラをロードしたが、どこにも表示されない

ディスプレイの解像度や配置を変更するとキャラクターが表示されなくなることがあります。

以下の手順で、表示位置をリセットします。

* コントロールパネル(※`ホーム`や`配信`タブがある方のウィンドウ)をつかみ、スクリーンの左上あたりに移動します。
* 設定ウィンドウを開いて`ウィンドウ`タブを表示し、`キャラクター位置のリセット`ボタンを押します。
    + この時点でキャラクターが見えたら、[2: 基本的な使い方](./get_started.html)に沿ってキャラクターの位置や視点を調整します。
* まだキャラクターが見えない場合、設定ウィンドウの`ウィンドウ`タブで`背景を透過`のチェックをオフにして、設定ウィンドウの横にキャラクターウィンドウが表示されるか確認します。
* 設定ウィンドウの`レイアウト`タブで`カメラ`の項目にある`位置をリセット`ボタンを押して、視点をリセットします。
    * キャラクターが表示されるのを確認したら、[2: 基本的な使い方](./get_started.html)に沿ってキャラクターの位置や視点を調整します。

以上の手順で改善しない場合、`4.2. 起動直後にVMagicMirrorが停止する`の方法をお試し下さい。

## 4.7. VMagicMirrorを起動したときのキャラの位置がおかしい

v0.8.1の不具合で確認しています。v0.8.2以降では修正されています。

## 4.8. 「VRMをロード」でキャラを選んでも何も動かない

セキュリティソフトが起動しているとコントロールパネル、キャラ表示ウィンドウの通信が失敗することがあります。

セキュリティソフトがインストールされ、動作している場合、無効にして動作するか確認してください。

事例として、COMODO Internet Securityの使用時にこの現象が起きることが報告されています。

## 4.9. 影が綺麗に映らない

* `Unlit`系シェーダーを使っているキャラの場合、映らないことがあります。
* VRoidStudio製のモデルなどで、服のテクスチャを部分的に透過している場合、本来は透明な部分が半透明で描画されてしまう事があります。

上記以外のケースでは、起動時設定でクオリティを上げると解決する場合があります(ただしCPU負荷が上昇します)。

* `VMagicMirror.exe`を起動するとき、通常のダブルクリックの代わりに`Shift`キーを押しながら`Enter`キーを打鍵することで、起動時設定のダイアログを表示します。
* `Quality Setting`の項目で`Very High`や`Ultra`を選択します。

上記で変更したクオリティ設定は、いちど設定すると次以降の起動時にも適用されます。

## 4.10. 「プレゼン風に右手を動かす」が有効なときの強調表示が邪魔

本機能はv0.8.6で追加されている機能です。

設定ウィンドウの`モーション`タブで「腕・ひじ」の項目にある`補助ポインターを表示`をオフにすると、強調表示がオフになります。

## 4.11. ゲームパッドを抜いたらVMagicMirrorがクラッシュした

ゲームプレイ後にゲームパッド(ゲームコントローラー)のケーブルを抜くとVMagicMirrorがクラッシュすることがあります。

この症状が起きたあと、VMagicMirrorを再起動しても繰り返しクラッシュしてしまう事があります。その場合、PCを再起動してください。

## 4.12. v0.9.3の使用時、VMagicMirrorコントロールパネルが起動しない

PC環境によって発生する場合があります。現在原因不明のため、もしこの症状があった場合は一つ手前のバージョン(v0.9.2)の使用を検討下さい。

## 4.13. v0.9.3の使用時、マウス感度が落ちる。

PC環境によって発生する場合があります。現在原因不明のため、もしこの症状があった場合は一つ手前のバージョン(v0.9.2)の使用を検討下さい。


## Sections

* [1: VMagicMirrorについて](./index.html)
* [2: 基本的な使い方](./get_started.html)
* [3: 詳細設定](./about_settings.html)
* 4: トラブルシューティング (このページ)
* [Tips A: デスクトップマスコット化のための設定](./tips_desktop_mascot.html)
* [Tips B: プレゼンテーションでVMagicMirrorを使う](./tips_presentation.html)
* [Tips C: 前バージョン(v0.8.0以降)の設定を引き継ぐ](./tips_load_prev_setting.html)
* [Tips D: キーボードやタッチパッドの見た目を変更する](./tips_change_textures.html)
* [License](./about_license.html)
* [Change Log](./changelog.html)
* [FAQ](./en_frequently_asked_questions.html)
