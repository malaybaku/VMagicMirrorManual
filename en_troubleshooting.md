
# 4. Troubleshooting

[Japanese](./troubleshooting.html)

## 4.1. Cannot click control panel or other application near to the character

Try to click and drag, and see if the character moves.

If the character moves, then move (s)he to far from the application you want to access, and then retry.

If the problem happens many times, then adjust the position and check off `(When Transparent) Drag character` in `Streaming` tab on control panel.

Please see [2: Getting Started](./en_get_started.html) > "2.3.1. Window" also.

## 4.2. VMagicMirror stops soon after started

Setting file might be broken in this case, so please try to reset the settings.

Open the folder in which `VMagicMirror.exe` exists, and then delete `_autosave` file in `ConfigApp` folder.

Then try to restatt.

### 4.3. Too high CPU usage

Set `Graphics Quality` to `High` when starting VMagicMirror.

**WARN:** In v0.8.0, some machine with `Medium` or lower setting drastically increases CPU usage. It is a known issue.

If the CPU usage continues to be high, then disable lip sync and face tracking on `Streaming` tab on control panel.

If you do not use game pad, then: 

* Open setting window by clicking `Open setting window` at `Home` tab in on control panel.
* Check off `Layout` > `GamePad` > `Enable Input Capture`.


## Sections

* [1: VMagicMirror](./en_index.html)
* [2: Getting Started](./en_get_started.html)
* [3: Settings](./en_about_settings.html)
* [4: Troubleshooting](./en_troubleshooting.html)
* [Tips A: Desktop Mascot Setup](./en_tips_desktop_mascot.html)
* [Tips B: VMagicMirror for Presentation](./en_tips_presentation.html)
* [License](./en_about_license.html)
