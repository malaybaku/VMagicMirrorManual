
# 4. Troubleshooting

[Japanese](./troubleshooting.html)

## 4.1. Cannot click control panel or other application near to the character

Try to click and drag, and see if the character moves.

If the character moves, then move (s)he to far from the application you want to access, and then retry.

If the problem happens many times, then adjust the position and check off `(When Transparent) Drag character` in `Streaming` tab on control panel.

Please see [2: Getting Started](./en_get_started.html) > "2.3.1. Window" also.

## 4.2. VMagicMirror stops soon after started

Setting file might be broken in this case, so please try to reset the settings.

* Press `Reset` on the control panel `Home` tab, and then press `OK` on the confirmation dialog to reset settings.
    + If it recovers the situation, please follow [2: Get Started](./en_get_started.html) to setup.
* If the problem still remains, exit VMagicMirror.
* Open the folder in which `VMagicMirror.exe` exists, and then delete `_autosave` file in `ConfigApp` folder. Then try to restatt.

### 4.3. Too high CPU usage

When you are using v0.8.0 or older, set `Graphics Quality` to `High` when starting VMagicMirror.

**WARN:** In v0.8.0, some machine with `Medium` or lower setting drastically increases CPU usage. It is a known issue.

If the CPU usage continues to be high, then disable lip sync and face tracking on `Streaming` tab on control panel.

If you do not use game pad, then: 

* Open setting window by clicking `Open setting window` at `Home` tab in on control panel.
* Check off `Layout` > `GamePad` > `Enable Input Capture`.


### 4.4. Eyes do not mouse pointer 

It is by specification, for some game software (please see detail in *note*).

Using fixed eye motion might improve appearance. 

* Control panel > `Streaming` tab > `Face` > `Eye Look Target` > select `None`


*note*: Cause of the trouble is as following.

Some game runs program to move mouse position to the center of game window. 

(FPS games need this type of program to support mouse-based camera control without getting unexpected mouse position.)

It results the fixed mouse position and eye / head position of character, even if you are moving mouse physically.

One example of the popular software which leads the trouble is VRChat Desktop Mode.


### 4.5. Eye Blink tracking does not work

If you put on glasses, try without them.

Some frame with thick frame prevents face tracking system.

If not, please check following points to help face tracking system.

* Proper distance from camera
* The room is bright
* Neck and face outline is clear
* Show mouth to the camera (*it is okay the microphone partly hide your mouth)

Showing entire face helps eye blink tracking, because face tracking system finds your face by detecting your whole face landmark points (including mouth, eyebrows, and of course eyes).

## Sections

* [1: VMagicMirror](./en_index.html)
* [2: Getting Started](./en_get_started.html)
* [3: Settings](./en_about_settings.html)
* [4: Troubleshooting](./en_troubleshooting.html)
* [Tips A: Desktop Mascot Setup](./en_tips_desktop_mascot.html)
* [Tips B: VMagicMirror for Presentation](./en_tips_presentation.html)
* [Tips C: Load Previous Version Setting](./en_tips_load_prev_setting.html)
* [License](./en_about_license.html)
* [Change Log](./en_changelog.html)