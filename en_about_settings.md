
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

`Window` also supports to fix the position after the application started, by following setup.

[![Fix Window Position](./images/about_settings/img01_015_fix_window_pos.png)](./images/about_settings/img01_015_fix_window_pos.png){: data-lightbox="img01_015"}

1. Follow [2: Getting Started](./get_started.html) to load character and move to anywhere you want to put.
2. Confirm that `Window` tab of the setting window is open.
3. Check on `Move window to specific position on startup`
4. Click `Check Current Window Position`
5. See the texts at the right of `X(Left = 0)` and `Y(Top = 0)` change to non-zero value.

If you want to try the result, quit the VMagicMirror and restart.

If the character does not appear, check on control panel `Home` tab > `Load current VRM on next startup`.

## 3.2. Motion

`Motion` tab can adjust character's proportion and motion related parameters.

[![Motion Tab](./images/about_settings/img01_018_motion_tab.png)](./images/about_settings/img01_018_motion_tab.png){: data-lightbox="img01_018"}

### 3.2.1. Face

Except the bottom item the properties are the same as `Streaming` tab in control panel.

The bottom item `Default Fun Blend Shape [%]` specifies the default fun expression rate.

As the value increases the character will become always smile, but some character's facial expression will be unnatural when combined to blink or other face motions.

In those cases, decrease the value.


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
* [License](./en_about_license.html)
