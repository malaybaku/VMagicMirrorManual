# Tips 2: デスクトップマスコット化のための設定

VMagicMirrorをデスクトップマスコット化するには次のようにします。

## Step 1: VMagicMirrorのセットアップ

* [1: キャラクターを読み込んで動かす](./get_started.html)の手順にしたがって、VRMを読み込み、背景の透明化などのセットアップをします。
* [Tips 1: 表示位置を固定する](./tips_fix_position.html)の手順にしたがって、キャラクターの表示位置を固定します。
* 設定ウィンドウの`ホーム`タブで、`次回の起動時にも同じVRMを読み込む`のチェックをオンにします。

以上の設定を行い、いったんVMagicMirrorを終了して再度起動します。

再起動前と同じ位置に、同じキャラクターが表示されれば成功です。


## Step 2: Windowsの起動時にVMagicMirrorをスタートさせる

Windowsを起動した直後に自動でVMagicMirrorをスタートするには以下のようにします。

* `VmagicMirror.exe`を右クリックし、ショートカットを作成します。
* Windowsのスタートアップフォルダの中へショートカットを移動します。

スタートアップフォルダのパスは通常、以下のようなフォルダになっています。

`C:\Users\(ユーザー名)\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup`

ドライブ名やユーザー名の部分は実際の環境にあわせて読み替えてください。

異なるバージョンのVMagicMirrorで置き換える場合や、Windows起動時にVMagicMirrorが起動する処理をやめたい場合、ショートカットを削除します。


* [VMagicMirror](./index.html)
* [1: キャラクターを読み込んで動かす](./get_started.html)
* [2: 詳細設定](./about_setttings.html)
* [3: トラブルシューティング](./troubleshooting.html)
* [Tips 1: 表示位置を固定する](./tips_fix_position.html)
* Tips 2: デスクトップマスコット化のための設定 (このページ)
* [Tips 3: プレゼンテーションでVMagicMirrorを使う](./tips_presentation.html)
