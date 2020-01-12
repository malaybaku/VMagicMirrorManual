
# Tips D: キーボードやタッチパッドの見た目を変更する

[English](./en_tips_change_textures.html)

※本機能はVMagicMirror 0.9.6以降で正式サポートとなりますが、それ以前のバージョンでも最低限動作します。

キーボードのキーや、タッチパッドの画像を好きなものに変更できます。`png`形式の画像のみをサポートしています。

画像を変更するためには、`VMagicMirror.exe`を起動する前に以下のフォルダを開きます。

`(VMagicMirror.exeのあるフォルダ)/VMagicMirror_Data/StreamingAssets`

このフォルダへ差し替えたい画像を追加します。ファイル名は次のようにしてください。

* キーボードのキー画像を差し替える場合: `key.png`
* タッチパッドの画像を差し替える場合: `pad.png`
* ゲームパッドの本体部分を差し替える場合: `gamepad_body.png`
* ゲームパッドのスティックやボタン部分を差し替える場合: `gamepad_button.png`

変更したい画像のみを差し替えることができます。

また、ゲームパッドに関しては単色画像での差し替えのみを想定しているため、イラストは適用しないで下さい。

画像を配置してから`VMagicMirror.exe`を実行することで、配置した画像が読み込まれます。

[![Change Texture](./images/tips/img_tips_10_change_texture.png)](./images/tips/img_tips_10_change_texture.png){: data-lightbox="img_tips_10"}

もとに戻したいときは、配置した`key.png`および`pad.png`を削除してからVMagicMirrorを再び起動します。

## Known issue

v0.9.4およびv0.9.5での既知の不具合として、キーボードやタッチパッドを表面から見たときと、裏面から見たときで、画像の向きが反転します。

v0.9.6時点で修正予定です。


## Sections

* [1: VMagicMirrorについて](./index.html)
* [2: 基本的な使い方](./get_started.html)
* [3: 詳細設定](./about_settings.html)
* [4: トラブルシューティング](./troubleshooting.html)
* [Tips A: デスクトップマスコット化のための設定](./tips_desktop_mascot.html)
* [Tips B: プレゼンテーションでVMagicMirrorを使う](./tips_presentation.html)
* [Tips C: 前バージョン(v0.8.0以降)の設定を引き継ぐ](./tips_load_prev_setting.html)
* Tips D: キーボードやタッチパッドの見た目を変更する (このページ)
* [License](./about_license.html)
* [Change Log](./changelog.html)
* [FAQ](./en_frequently_asked_questions.html)
