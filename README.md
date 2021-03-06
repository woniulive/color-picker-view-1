# ColorPickerView
This component is forked from danielnilsson9,you can visit https://github.com/danielnilsson9/color-picker-view to see detail information.I forked it so that i can edit because it seems that daniel nilsson don't maintain it anymore.The pull request of andre99 don't have any response,i add it by myself.
##### A simple good looking color picker component for Android

A color picker is something that has always been missing from the standard set of components which developers can build their user interface in Android with. This is a color picker which I wrote for one of my own project which I decided to release as open source.

### Screenshots
<img src="https://github.com/woniulive/color-picker-view/blob/d11cbbe9862642128aa62f303d4d8b6f22e0b611/demo/phone_screenshot.png" alt="Screenshot1" width="240">
<img src="https://github.com/woniulive/color-picker-view/blob/d11cbbe9862642128aa62f303d4d8b6f22e0b611/demo/tablet_screenshot.png" alt="Screenshot2" width="460">

### How to use
The library is on jcenter. If you are using Android studio (and gradle), just add this line to your module
build.gradle file under dependencies:

````gradle
dependencies {
    compile "com.github.danielnilsson9:color-picker-view:1.4.0@aar"
}
````

For doumentation about how to use the library, check the demo app included in this project.

There are basicly three different ways to use this color picker. You can add it to your preferences using the ColorPreference class. You can also use it as a DialogFragment using the ColorPickerDialogFragment. Or you can simply use the ColorPickerView to add the color picker anywhere you want in you application. All three cases are demonstrated in the demo app, please refer to the demo for more information.

### Changelog
##### Version 1.5.0
- Add support for hexadecimal input(Thanks andre99)

##### Version 1.4.0
- Change of package name due to problem with jcenter publish. New package name is: com.github.danielnilsson9.colorpickerview, sorry for the inconvenience.
- Fix for project could not be built due to obsolet android build tool version used.

##### Version 1.3.0
- Bugfix: Selected Hue value in hue panel did not perfectly match what was shown in in the Saturation/Value panel.
- Bugfix: Layout issues on sw320dp displays.
- Bugfix: Title could not be changed or removed in ColorPickerDialogFragment.

##### Version 1.2.0
- Api level 13 (Android 3.2) is now required by the library.
- The ColorPickerDialog which was based on an AlertDialog has been replaced by ColorPickerDialogFragment which is based on a DialogFragment.
- New layout on the color picker dialog, should look good on all screen sizes and orientations.
- ColorPickerPreferences was replaced by ColorPreference. The ColorPreference does NOT take care of showing the ColorPickerDialogFragment, you will have to do that yourself, see the demo app. This is due to the fact that we don't have access to the fragment manager from the Preference class.
- ColorPickerView now automatically saves it state on orientation change etc.
