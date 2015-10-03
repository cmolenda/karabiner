# karabiner-win-on-mac
Configurations for Windows Keyboards on Mac via Karabiner private.xml files. This is not actively maintained and only has a couple of incomplete configuration files for some Windows based ergonomic keyboards that I've used in the past.
* OysterErgonomics UltraErgo
* Kinesis Freestyle2

## Install
1. Make sure you've installed and are running the latest version of Karabiner: https://pqrs.org/osx/karabiner/
2. Copy this repo to your local Mac
  ```
  git clone git@github.com:cmolenda/karabiner-win-on-mac.git ~/Library/Application\ Support/Karabiner/karabiner-win-on-mac/
  ```
3. Add this line to your `~/Library/Application\ Support/Karabiner/private.xml` anywhere between the opening `<root>` and closing `</root>` tags.
  ```
    <include path="karabiner-win-on-mac/_keyboards.xml" />
  ```
     Alternatively, you can add individual keyboard files like so:
  ```
    <include path="karabiner-win-on-mac/oysterergonomics_ultraergo.xml"
  ```
4. Reload your XML
  1. Open Karabiner
  2. Right click the icon for Karabiner in your toolbar
  3. Click Preferences
  4. Select the Change Key tab
  5. Click Reload XML
5. Under `remapping`, select the keyboard that you're using.
6. (Optional Recommended) Under `Karabiner core settings > Exclude devices` select:
  * `Don't remap an internal keyboard`
  * `Don't remap Apple's keyboards`
  * `Don't remap Apple's pointing devices`
