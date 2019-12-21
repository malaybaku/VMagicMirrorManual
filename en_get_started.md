
# 2: Getting Started

[Japanese](./get_started.html)

## 2.1. Start and Exit VMagicMirror

`VMagicMirror.exe` is main .exe file of VMagicMirror.

When you start the application you will see "Control Panel" with GUI and "Character Window", where the character will appear.

[![Start Image](./images/get_started/img00_015_started.png)](./images/get_started/img00_015_started.png){: data-lightbox="img00_015"}

When you close one of control panel or character window, then the other window will automatically close and VMagicMirror shuts down.

Instead, the control panel can be minimized during you do not need it.

## 2.2. Load Character

<iframe 
    width="560" 
    height="315" 
    src="https://www.youtube.com/embed/I-CHfCHbjx8?autoplay=1&loop=1&playlist=I-CHfCHbjx8" 
    frameborder="0" 
    allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
</iframe>

In the control panel `Home` tab, select `Load VRM` button to select `.vrm` file on your PC.

[![Load VRM](./images/get_started/img00_020_load_vrm.png)](./images/get_started/img00_020_load_vrm.png){: data-lightbox="img00_020"}

After you selected the character the license will be shown.

[![Load Confirmation](./images/get_started/img00_030_load_vrm_confirmation.png)](./images/get_started/img00_030_load_vrm_confirmation.png){: data-lightbox="img00_030"}

**NOTE:** If you cannot see the license and you are using some security software, please retry after disabling them.

After the confirmation and `OK`, then the character will appear and react to your mouse and keyboard input.

If you want to use the same character every time, check `Load current VRM on next startup`.

[![After Loaded](./images/get_started/img00_040_after_loaded.png)](./images/get_started/img00_040_after_loaded.png){: data-lightbox="img00_040"}

**Hint:** If your character and keyboard / mouse layout do not match, do not worry. First you can use `Adjust size by VRM` button to fix camera positions and keyboard / mouse pad positions. 

[![Not Adjusted Layout](./images/get_started/img00_160_not_good_layout_example.png)](./images/get_started/img00_160_not_good_layout_example.png){: data-lightbox="img00_160"}

[![After Adjusted](./images/get_started/img00_170_after_adjust.png)](./images/get_started/img00_170_after_adjust.png){: data-lightbox="img00_170"}

Also you can see about more detailed customize in section [3: Settings](./en_about_settings.html).

## 2.3. Streaming 

From `Streaming` tab in control panel, you can access to all main features in VMagicMirror.

After loading VRM please try them.

[![Streaming Tab](./images/get_started/img00_050_streaming_tab.png)](./images/get_started/img00_050_streaming_tab.png){: data-lightbox="img00_050"}

### 2.3.1. Window

Check on `Window` > `Transparent Window` then the character window's background becomes transparent. It is good to use VMagicMirror normally in this state.

[![Transparent Background](./images/get_started/img00_060_transparent_bg.png)](./images/get_started/img00_060_transparent_bg.png){: data-lightbox="img00_060"}

After setup transparent background, then confirm to check `(When Transparent) Drag the character`. You can left-click and drag the character during the check is on.

[![Transparent Background](./images/get_started/img00_070_transparent_bg_drag.png)](./images/get_started/img00_070_transparent_bg_drag.png){: data-lightbox="img00_070"}

However the `Drag the character` check might prevent your mouse input.

So, please check off `(When Transparent) Drag the character` after you have moved the character to the position you like.

[![Transparent BG can click](./images/get_started/img00_090_transparent_bg_can_click.png)](./images/get_started/img00_090_transparent_bg_can_click.png){: data-lightbox="img00_090"}


### 2.3.2. Face

`Face` can setup your VRM's face expressions.

[![Face Streaming](./images/get_started/img00_100_streaming_face.png)](./images/get_started/img00_100_streaming_face.png){: data-lightbox="img00_100"}

#### LipSync

Check on `LipSync` and select microphone device, then lipsync is available.

#### Track Face

Check on `Track Face` and select camera to enable face tracking.

If your face is not at the center for the web camera, or you are too near/far to the camera, the character indication might be unnatural. In this case, click `Calibrate position` to adjust.

**Hint:** When you use v0.9.3 or older version, and if your character have always closing eye, try to close your eye halfly and `Calibrate position`, then the character tends to open eyes. Similarly, when your character always look downward then look down and `Calibrate position` to adjust.


#### Eye Look Target

In default, VMagicMirror setup makes character to look at mouse.

This motion is suited for working streaming or presentation, but you might needs other type of motions.

* Mouse (Default): Character looks at mouse pointer position.
* User : Character always look at you. You can use it when the `Mouse` option too much moves character's eyes.
* None : Eye Look Target is always forward to the character's head. In this mode you can move the neck by face tracking, but eye will not move in most cases.

### 2.3.3. Word To Motion

"Word to Motion" is the feature to support motion and face expression with your custom, and you can test its default expression set here.

[![Word to Motion](./images/get_started/img00_105_word_to_motion.png)](./images/get_started/img00_105_word_to_motion.png){: data-lightbox="img00_105"}

Confirm `Enable Word to Motion` is on, and you can launch face expression by one of following ways.

* Type word "joy", "angry", "sorrow", or "fun".
* Select `Gamepad` from `Assign device for this function` , and press A, B, X, or Y button.
* Select `Keyboard` from `Assign device for this function` , and press 1, 2, 3, or 4 key.

Please see the detail at "3.5. Word to Motion" in [3: Settings](./en_about_settings.html).

**NOTE:** If you select keyboard or gamepad for `Assign device for this function`, then the character ignores the selected device as arm motion input. 

For example, if you select keyboard the character stops typing motion. The following concept will help which one you should use.

* Case to select `None`: Not streaming purpose, but for desktop mascot.
    - `None` selection reflects both keyboard and gamepad input to arm motion, so the character's motion will look like most similar as yours.
* Case to select `Gamepad`: Share your screen, with some working like writing or painting.
    - You can keep the character looking to work with keyboard/mouse, while you can change the face expression by gamepad.
* Case to select `Keyboard`: Stream the game play.
    - You can keep the character looking to play game with gamepad, while you can change the face expression by keyboard.

### 2.3.4. View

Toggle `Keyboard`, `Gamepad` or `Avatar's Shadow` to show and hide them.

[![Keyboard Visible](./images/get_started/img00_110_view_keyboard_visible.png)](./images/get_started/img00_110_view_keyboard_visible.png){: data-lightbox="img00_110"}

[![Keyboard Hidden](./images/get_started/img00_120_view_keyboard_hidden.png)](./images/get_started/img00_120_view_keyboard_hidden.png){: data-lightbox="img00_120"}

*In v0.9.0-v0.9.4, gamepad is always disappeared.

**Hint:** If the shadow looks not good, please refer to [4: Troubleshooting](./en_troubleshooting.html) and see "4.9. Shadow looks not good". If this troubleshooting does not work well, please disable shadow.

`Typing Effect` is enabled when you select `text` option at the center, or `light` at the right.

[![Typing Effect](./images/get_started/img00_125_view_typing_effect_example.png)](./images/get_started/img00_125_view_typing_effect_example.png){: data-lightbox="img00_125"}


### 2.3.5. Camera

This "Camera" means eyesight on the character window.

You can set the camera to see the character from any direction you want, by `Free Camera Mode`.

Before using this feature, disable `Window` > `Transparent Window` temporary.

Check on `Free Camera Mode` and click character window.

Then, during the character window is active, you can move the camera by following inputs.

* Right click + drag : rotate camera
* Middle click + drag : translate camera to up/down/left/right
* Middle wheel : move camera forward or backword.

[![Free Camera Mode](./images/get_started/img00_130_free_camera_mode.png)](./images/get_started/img00_130_free_camera_mode.png){: data-lightbox="img00_130"}

When you lost the character in window or you want to reset, click `Reset Position`.

After adjusting the camera check on `Transparent Window` again.

Similar to `Drag character`, the `Free Camera Mode` may leads wrong operation to change the camera position, so please check off `Free Camera Mode` after finishing the adjust.

[![After Free Camera Mode](./images/get_started/img00_140_after_free_camera_mode.png)](./images/get_started/img00_140_after_free_camera_mode.png){: data-lightbox="img00_140"}

From v0.9.4, camera quick save / load is supported.

Setup the view by `Free Camera Mode`, and click one of `[1], [2], or [3]` button to save the camera setting. After saving, you can load them by `Quick Load` buttons.

[![Camera Quick Save](./images/get_started/img00_135_camera_quick_save.png)](./images/get_started/img00_135_camera_quick_save.png){: data-lightbox="img00_135"}


**Hint:** Actually you can set camera position with transparent window also.

* Check on `(When Transparent) Drag Character`
* Left click the character
* Adjust camera position
* After adjusting, check off `(When Transparent)Drag Character`

**Note:** If you follow the way above, the character might be partially cut off by going out to character window. If you lost the character and want to reset, then press `Reset Position` button, or check off `Transparent Window` to see what is happening.

### 2.3.6. Device Layout

This feature is available from v0.9.5.

Turn on `Free Layout` to enter device free layout mode.

[![Device Free Layout](./images/get_started/img00_200_free_layout.png)](./images/get_started/img00_200_free_layout.png){: data-lightbox="img00_200"}

When enter this mode `Transparent Window` is turned off.

During this mode, character window shows UI on the top-left.

* Control Mode: Choose which parameter to change, position, rotation, or scale.
* Coordinate: Choose the coordinate from device local, or world. If you are not clear about this, use `Local`.
* Gamepad Scale: Adjust gamepad model size. If gamepad is too big for your avatar, then decrease this value.

`Reset` can recover the standard layout.


### 2.3.7. Motion

Check on `Presentation-like hand` to move VRM's right hand as if he / she is on a presentation.

[![Presentation Mode](./images/get_started/img00_150_presentation_mode.png)](./images/get_started/img00_150_presentation_mode.png){: data-lightbox="img00_150"}

This style matches when you have presentation or you want to create instruction video.

When quitting the mode check off `Presentation-like hand`.

**Hint:** Detail is in [Tips B: VMagicMirror for Presentation](./en_tips_presentation.html).

### 2.3.8. Screenshot

[![Screenshot](./images/get_started/img00_180_screenshot.png)](./images/get_started/img00_180_screenshot.png){: data-lightbox="img00_180"}

Press `Take` button to start 3 second count down, and the screenshot will be captured.

Screenshot is saved to the `Screenshots` folder in the folder where `VMagicMirror.exe` exists.

The screenshot is transparent considered image. If you turn on shadow it will be also included. This S

[![Screenshot Result](./images/get_started/img00_190_screenshot_shadow.png)](./images/get_started/img00_190_screenshot_shadow.png){: data-lightbox="img00_190"}


## 2.4. For further customize

You may see some problems about the looking of your VRM.

* Keyboard position is too high or low for my character...
* The character looks too bright or too dark...

In this case [3: Settings](./en_about_settings.html) will solve your problems, so please refer to them.

## Sections

* [1: VMagicMirror](./en_index.html)
* 2: Getting Started (this page)
* [3: Settings](./en_about_settings.html)
* [4: Troubleshooting](./en_troubleshooting.html)
* [Tips A: Desktop Mascot Setup](./en_tips_desktop_mascot.html)
* [Tips B: VMagicMirror for Presentation](./en_tips_presentation.html)
* [Tips C: Load Previous Version Setting](./en_tips_load_prev_setting.html)
* [Tips D: Change Device Textures](./en_tips_change_textures.html)
* [License](./en_about_license.html)
* [Change Log](./en_changelog.html)
* [FAQ](./en_frequently_asked_questions.html)
