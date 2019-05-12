
# 3. Settings

[Japanese](./about_settings.html)

Setting Window is available from `Open Setting Window` on `Home` tab in control panel.

[![Setting Window](./images/about_settings/img01_010_setting_window.png)](./images/about_settings/img01_010_setting_window.png){: data-lightbox="img01_010"}

Setting Window supports detailed customization options.

* 3.1. `Window`
    - Character window control
* 3.2. `Motion`
    - Adjust character size related parameters and motion scale
* 3.3. `Layout`
    - Layout of the camera, keyboard, mouse pad, and gamepad
* 3.4. `Light`
    - Light and Bloom
    

## 3.1. Window

`Window` tab supports BG color when the character window is not transparent, and also can toggle whether the window is always foreground or not.

**Note:** From v0.8.1, the character position is automatically saved, so when you quit the application and restart, the character will appear at the same place as previous time.

**Hint:** When you lost where the character is, then turning off `Transparent Window` and pressing `Reset Character Position` might be a help.

## 3.2. Motion

`Motion` tab can adjust character's proportion and motion related parameters.

[![Motion Tab](./images/about_settings/img01_018_motion_tab.png)](./images/about_settings/img01_018_motion_tab.png){: data-lightbox="img01_018"}

### 3.2.1. Face

Upper part is the same as `Streaming` tab in control panel.

The item `Default Fun Blend Shape [%]` specifies the default fun expression rate.

As the value increases the character will become always smile, but some character's facial expression will be unnatural when combined to blink or other face motions. In those cases, decrease the value.

The `Eyebrow (Open to Customize)` is very advanced section and normally you do not need modify them. However if you have original VRM and want to move the eyebrow, or in case the eyebrow motion is too big or too small. 

* This section requires the knowledge about `BlendShape` to control VRM facial expression. If you do not know well, please refer to [Virtual Cast Wiki](https://virtualcast.jp/wiki/doku.php?id=%E3%83%A2%E3%83%87%E3%83%AB%E4%BD%9C%E6%88%90:%E3%83%96%E3%83%AC%E3%83%B3%E3%83%89%E3%82%B7%E3%82%A7%E3%82%A4%E3%83%97%E8%A8%AD%E5%AE%9A) and see latter section's image. You will see the name like `mouth_a` or `mouth_b`. This is BlendShape. And you can specify the name of BlendShape to move eyebrow, by sliding each shape in Unity Editor.


### 3.2.2. Arm

Setup how to move the arm.

`Waist width [cm]`and `Strength to keep upper arm to body [%]` are the parameters to keep the elbow close to body(, which is subtle but critical for the cute motion).

Please see the following example of default value, close elbow strongly, and open.

[![Arm Side Default](./images/about_settings/img01_020_arm_side_default.png)](./images/about_settings/img01_020_arm_side_default.png){: data-lightbox="img01_020"}

[![Arm Side Close](./images/about_settings/img01_030_arm_side_close.png)](./images/about_settings/img01_030_arm_side_close.png){: data-lightbox="img01_030"}

[![Arm Side Open](./images/about_settings/img01_040_arm_side_open.png)](./images/about_settings/img01_040_arm_side_open.png){: data-lightbox="img01_040"}

`Presentation-like motion scale [%]` has effect during `Presentation-like hand` check is on.

The value should be small when the character is enough small compared to the whole monitor size to avoid the right arm always stretched, or vise versa.

`Arm position radius min [cm]` helps to avoid arm going into the body, when large value is set. However too large value makes the arm always stretched.

### 3.2.3. Hand

Parameters about hand or finger length and typing motion.

Check those values when the typing motion is done far from the keyboard, or the hand is too float above the keyboard.

**Hint:** After setup natural motion, set large value to `(Press key) Hand height adjust [cm]`, which make comical big typing motion.

[![Large Typing Motion](./images/about_settings/img01_045_large_type_motion.png)](./images/about_settings/img01_045_large_type_motion.png){: data-lightbox="img01_045"}


### 3.2.4. Wait motion

Wait motion is breathing like motion.

It might be helpful for some characters to show as if (s)he is floating, with large `Scale [%]` and short `Period [sec]`.


## 3.3. Layout

In `Layout` tab you can access to the parameters to adjust surrounding device layout like camera, keyboard, mouse pad, and gamepad.

[![Layout Tab](./images/about_settings/img01_050_layout_tab.png)](./images/about_settings/img01_050_layout_tab.png){: data-lightbox="img01_050"}

### 3.3.1. Camera

Same as `Camera` menu in control panel `Streaming` tab.

### 3.3.2. Keyboard

You can change the size and height of the keyboard and mouse pad, along to your character's scale.

### 3.3.3. Gamepad

Similar top the keyboard, height and size is adjustable.

For the gamepad, the character leans by the stick input. If you have a gamepad, let's check it by moving left stick with default setting!

* In `Lean by stick` list you can select what stick (or direction key) the character should be react.
* `Reverse direction to lean` support to lean reversed direction.

**NOTE:**

In default the gamepad feature is available, but if you do not use it, and the VMagicMirror performance is not good on your machine, then check off `Enable Input Capture` on the top of `Gamepad` menu.


## 3.4. Light

In `Light` tab you can set the light and bloom colors and intensities.

**NOTE:** Please be aware that some VRM character uses `Unlit` type shader, to which the light setting has no effect.


## Sections

* [1: VMagicMirror](./en_index.html)
* [2: Getting Started](./en_get_started.html)
* 3: Settings (this page)
* [4: Troubleshooting](./en_troubleshooting.html)
* [Tips A: Desktop Mascot Setup](./en_tips_desktop_mascot.html)
* [Tips B: VMagicMirror for Presentation](./en_tips_presentation.html)
* [Tips C: Load Previous Version Setting](./en_tips_load_prev_setting.html)
* [License](./en_about_license.html)
* [Change Log](./en_changelog.html)