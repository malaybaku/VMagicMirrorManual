
# Tips A: デスクトップマスコット化のための設定

[English](./en_tips_desktop_mascot.html)

VMagicMirrorはデスクトップマスコット化としても使えます。

本セットアップによって、Windowsの起動後に、所定の位置へキャラクターを表示できます。

## Tips A.1. VMagicMirrorのセットアップ

* [2: 基本的な使い方](./get_started.html)の手順にしたがってVRMを読み込み、背景の透明化などのセットアップをします。
* [3: 詳細設定](./about_settings.html)のうち"3.1. ウィンドウ"に記載された手順にしたがって、キャラクターの表示位置を固定します。
* コントロールパネルの`ホーム`タブで、`次回の起動時にも同じVRMを読み込む`のチェックがオンになっている事を確認します。

以上ののち、いったんVMagicMirrorを終了して再び起動します。

終了前と同じ位置にキャラクターが表示されれば成功です。


## Tips A.2. Windows起動時にVMagicMirrorをスタート

コントロールパネルの`ホーム`タブ左下にある、`Windowsの起動後にスタート`のチェックをオンにします。

また、もしVMagicMirror v0.8.0以前のバージョンでショートカットをスタートアップフォルダに配置していた場合、削除します。スタートアップフォルダは以下のようなフォルダですが、ドライブ名やユーザー名の部分は実際の環境にあわせて読み替えてください。

`C:\Users\(ユーザー名)\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup`

以上のセットアップ後にWindowsを再起動してみて、VMagicMirrorが表示されれば成功です。

もし将来的に異なるバージョンのVMagicMirrorで置き換える場合や、自動で立ち上がる設定を無効にしたい場合、`Windowsの起動後にスタート`のチェックをオフにします。


## Sections

* [1: VMagicMirrorについて](./index.html)
* [2: 基本的な使い方](./get_started.html)
* [3: 詳細設定](./about_settings.html)
* [4: トラブルシューティング](./troubleshooting.html)
* Tips A: デスクトップマスコット化のための設定 (このページ)
* [Tips B: プレゼンテーションでVMagicMirrorを使う](./tips_presentation.html)
* [Tips C: 前バージョン(v0.8.0以降)の設定を引き継ぐ](./tips_load_prev_setting.html)
* [License](./about_license.html)
* [Change Log](./changelog.html)
* [FAQ](./en_frequently_asked_questions.html)
