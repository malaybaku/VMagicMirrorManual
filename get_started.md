
# 2: 基本的な使い方

[English](./en_get_started.html)

## 2.1. VMagicMirrorの開始と終了

`VMagicMirror.exe`を起動すると、GUIがある「コントロールパネル」と、キャラクターが映る「キャラクター表示ウィンドウ」が立ち上がります。

[![Start Image](./images/get_started/img00_015_started.png)](./images/get_started/img00_015_started.png){: data-lightbox="img00_015"}

コントロールパネルかキャラクター表示ウィンドウの一方を閉じると、もう片方の画面も閉じてVMagicMirrorが終了します。「キャラクターは表示したいがコントロールパネルは隠したい」という場合、コントロールパネルを最小化します。


※v0.8.0では解像度の選択ダイアログを表示していましたが、v0.8.1では廃止しています。その代わりに、キャラクターウィンドウを直接引き延ばしてサイズを調整できます。


## 2.2. キャラクターの表示

コントロールパネルの`ホーム`タブ内にある`VRMロード`ボタンを押し、PC上の`.vrm`ファイルを選択します。

[![Load VRM](./images/get_started/img00_020_load_vrm.png)](./images/get_started/img00_020_load_vrm.png){: data-lightbox="img00_020"}

キャラクターを選択すると、キャラクター表示ウィンドウに規約が表示されます。

[![Load Confirmation](./images/get_started/img00_030_load_vrm_confirmation.png)](./images/get_started/img00_030_load_vrm_confirmation.png){: data-lightbox="img00_030"}

確認して問題なければ`OK`をクリックすると、キャラクターが表示され、マウスやキーボードの操作に応じて動きます。

同じキャラクターを次回以降も使いたい場合、`VRMロード`ボタンの下にある、`次回の起動時にも同じVRMを読み込む`のチェックをオンにします。

[![After Loaded](./images/get_started/img00_040_after_loaded.png)](./images/get_started/img00_040_after_loaded.png){: data-lightbox="img00_040"}

**Hint:** キーボードやマウスの位置がキャラクターの体型からずれていますか？もしそうであれば、とりあえず`キャラの体型で補正`ボタンを押すことでレイアウトが調整されます。さらに調整する場合は、順に読み進めて[2: 詳細設定](./about_settings.html)のなかで調整できます。

## 2.3. 配信タブ

コントロールパネルの`配信`タブではVMagicMirrorのすべての主要機能にアクセスできます。

VRMをロードしたら、各機能を試してみましょう。

[![Streaming Tab](./images/get_started/img00_050_streaming_tab.png)](./images/get_started/img00_050_streaming_tab.png){: data-lightbox="img00_050"}

### 2.3.1. ウィンドウ

`ウィンドウ`で、`背景を透過`のチェックをオンにすることで、キャラクター表示ウィンドウの背景を透明にできます。VMagicMirrorは通常、この状態で使用します。

[![Transparent Background](./images/get_started/img00_060_transparent_bg.png)](./images/get_started/img00_060_transparent_bg.png){: data-lightbox="img00_060"}

背景を透明にしたとき、`(透過中)キャラ付近を掴んでドラッグ`のチェックがオンになっていれば、キャラクター付近を左クリック+ドラッグしてキャラクターを移動できます。

[![Transparent Background](./images/get_started/img00_070_transparent_bg_drag.png)](./images/get_started/img00_070_transparent_bg_drag.png){: data-lightbox="img00_070"}

ただし、`(透過中)キャラ付近を掴んでドラッグ`がオンのままだとキャラクターを誤って移動してしまったり、キャラクター背後のアプリケーションにアクセスできなくなったりします。

一見すると何もないエリアに、透明なキャラクター表示ウィンドウの当たり判定が存在するためです。

[![Transparent BG cannot click](./images/get_started/img00_080_transparent_bg_cannot_click.png)](./images/get_started/img00_080_transparent_bg_cannot_click.png){: data-lightbox="img00_080"}

この問題を防ぐためには、キャラクターを移動させたあとで`(透過中)キャラ付近を掴んでドラッグ`のチェックをオフにします。

すると、キャラクター表示ウィンドウがクリックに反応しなくなり、背後のウィンドウにもアクセスできます。

[![Transparent BG can click](./images/get_started/img00_090_transparent_bg_can_click.png)](./images/get_started/img00_090_transparent_bg_can_click.png){: data-lightbox="img00_090"}


**Hint:** VMagicMirrorでは、起動時にいつも同じ場所へキャラクターを配置することもできます。([3: 詳細設定](./about_settings.html)の"3.1. ウィンドウ"を参照下さい)


### 2.3.2. 顔・表情

`顔・表情`メニューはその名の通り、顔の動きに関連する主要な機能です。

[![Face Streaming](./images/get_started/img00_100_streaming_face.png)](./images/get_started/img00_100_streaming_face.png){: data-lightbox="img00_100"}

#### リップシンク

`リップシンク`はマイクを使用する機能です。このチェックをオンにし、右のマイク一覧から使いたいマイクを選ぶと、リップシンクが有効になります。

#### 顔トラッキング

`顔をトラッキング`ではウェブカメラが必要です。リップシンクと同様に、`顔をトラッキング`のチェックをオンにし、右の一覧からウェブカメラを選ぶことで、顔トラッキングが有効になります。

もしあなたの顔がカメラの正面から上下左右にずれていたり、カメラとの距離が近い、または遠い場合はキャラクターの姿勢がおかしくなるかもしれません。

その場合、普段の姿勢で画面を見つめて目を開き、`姿勢・表情を補正`ボタンをクリックします。補正に成功すると、キャラクターが中央に戻ります。

**Hint:** キャラクターの目が閉じがちになってしまう場合、目を半閉じにして`姿勢・表情を補正`ボタンをクリックすると、目が開きやすくなります。似たように、キャラクターがうつむきがちになる場合は、少し下を向いて`姿勢・表情を補正`ボタンをクリックすると、キャラが上を向くようになります。

**!注意!** VMagicMirror v0.8.0の時点では、一部のカメラを使うと極端に動作が遅くなる不具合を確認しています。そうなってしまった場合、顔トラッキングを無効化してください。


#### 視線の動き

VMagicMirrorの基本設定では、キャラクターがマウスポインタの方向を向きます。

これは作業配信やプレゼンテーションを想定したデフォルト設定ですが、都合によっては他のモードを選ぶこともできます。

* マウス: キャラクターはマウスポインタの方向を向きます。デフォルト設定です。
* ユーザー: キャラクターは常にあなたの方向を向きます。マウスの動きが激しすぎる場合などに使用します。
* 固定: 顔トラッキングのみで首を動かすようにします。動きをおさえたい場合に使用します。

### 2.3.3. 表示

`表示`から`キーボード・マウスパッド`や`ゲームパッド`のチェックのオン・オフを切り替えることで、これらの要素を表示するか隠すかを選択できます。

[![Keyboard Visible](./images/get_started/img00_110_view_keyboard_visible.png)](./images/get_started/img00_110_view_keyboard_visible.png){: data-lightbox="img00_110"}

[![Keyboard Hidden](./images/get_started/img00_120_view_keyboard_hidden.png)](./images/get_started/img00_120_view_keyboard_hidden.png){: data-lightbox="img00_120"}

### 2.3.4. カメラ

`フリーカメラモード`を用いるとカメラの視点を変更し、自由な方向からキャラクターを見られます。

本機能を使うときは、いったん`ウィンドウ`メニューの`背景を透過`をオフにします。

`フリーカメラモード`のチェックをオンにし、キャラクター表示ウィンドウを左クリックしてアクティブにします。

キャラクター表示ウィンドウがアクティブな間、いくつかの方法で視点を動かせます。

* 右クリック + ドラッグ : 視線を上下左右に回転
* 中クリック + ドラッグ : カメラを上下左右に平行移動
* 中ホイール : カメラを前後に移動

[![Free Camera Mode](./images/get_started/img00_130_free_camera_mode.png)](./images/get_started/img00_130_free_camera_mode.png){: data-lightbox="img00_130"}

キャラクターを見失った場合や、始めからやり直したい場合は、`位置をリセット`ボタンで初期状態に戻せます。

調整が終わったら`背景を透過`をふたたびオンにします。

また、`フリーカメラモード`も有効なままにすると誤ってカメラを動かしてしまう場合があるため、`フリーカメラモード`のチェックもオフにしておきます。

[![After Free Camera Mode](./images/get_started/img00_140_after_free_camera_mode.png)](./images/get_started/img00_140_after_free_camera_mode.png){: data-lightbox="img00_140"}

**Hint:** 操作に慣れてきたら、`背景を透過`をオンにしたままでも`フリーカメラモード`を使えます。

* `(透過中)キャラ付近を掴んでドラッグ`をオンにする
* キャラクターを左クリックする
* 右クリック、中クリック、ホイールで視点を調整
* キャラクターを動かしたくない場合、調整が終わりしだい`(透過中)キャラ付近を掴んでドラッグ`をオフにする

※`背景を透過`をオンにしたまま`フリーカメラモード`を用いると、気づかないうちにキャラクターがキャラクター表示ウィンドウから見切れることがあります。キャラクターが見切れてよく分からなくなってしまった場合は`位置をリセット`ボタンを押してやり直す、`背景を透過`をオフにしてウィンドウの位置を確認します。

### 2.3.5. モーション

`プレゼン風に右手を動かす`のチェックをオンにしてマウスを動かすと、キャラクターが右手でマウスポインタの方向を指し示します。

[![Presentation Mode](./images/get_started/img00_150_presentation_mode.png)](./images/get_started/img00_150_presentation_mode.png){: data-lightbox="img00_150"}

このスタイルは解説動画やプレゼンテーションでVMagicMirrorを使うときに有効です。

このモードを終了するときは`プレゼン風に右手を動かす`のチェックをオフにします。

**Hint:** 詳しくは[Tips B: プレゼンテーションでVMagicMirrorを使う](./tips_presentation.html)もあわせてご覧下さい。


## 2.4. もっと細かく調整したい方へ

ここまで動かしてみて、見た目に気になる点があった方もいると思います。

* キーボードの位置がキャラクターに比べて高すぎ・低すぎ
* キャラクターが明るすぎる・暗すぎる

[3: 詳細設定](./about_settings.html)ではこれらの問題を解決できます。

個々のキャラクターにあわせてしっかりと調整したい方はこちらもお読みください。

## Sections

* [1: VMagicMirrorについて](./index.html)
* 2: 基本的な使い方 (このページ)
* [3: 詳細設定](./about_settings.html)
* [4: トラブルシューティング](./troubleshooting.html)
* [Tips A: デスクトップマスコット化のための設定](./tips_desktop_mascot.html)
* [Tips B: プレゼンテーションでVMagicMirrorを使う](./tips_presentation.html)
* [Tips C: 前バージョン(v0.8.0以降)の設定を引き継ぐ](./tips_load_prev_setting.html)
* [License](./about_license.html)
