# MacOS

Tools, notes, and shared packages for [MacOS](https://www.apple.com/macos).

## Setup
### System Settings
* General -> Appearance -> Auto
* Desktop & Screen Saver -> Fliqlo (install via homebrew)
  * Start after: 5 Minutes
  * Scale: 85%
* Dock
  * Turn Hiding Off
  * Turn Maginification Off
  * Resize Dock
* Mission Control
  * Disable `Automatically rearrange Spaces based on most recent use`
  * Disable `When switching to an application, switch to a Space with open windows for the application`
  * Disable `Group windows by application`
* Siri -> Disable
* Spotlight -> Disable Allow Spotlight Suggestions in Look up
* Keyboard
  * Modifier Keys -> Caps Lock to Escape
  * Set Key Repeat to Fastest
  * Decrease Delay Until Repeat 1 tick from middle default
  * Remove default Text expansions
  * Shortcuts
    * Disable Turn Dock Hiding On/Off
    * Enable Switch to Desktop 1 - 6
    * Change Switch to Desktop 1 - 6 modifier from ctrl to alt
    * Enable Move focus to active or next window
    * Enable Show Spotlight search
  * Dictation -> Off
* Trackpad
  * Enable Tap to click
  * Disable 2 Finger Secondary click
  * Increase Tracking Speed 1 tick from middle default
  * More Gestures
    * Swipe Between pages: 2 Fingers
    * Swipe between full-screen apps: 4 Fingers
    * Mission Control: Swipe up 4 Fingers
    * App Expose: Swipe down 4 Fingers
    * Disable any Gesture that uses 3 Fingers
* Display
  * Scaled to More Space
  * Night Shift -> Sunset to Sunrise
* Energy Saver
  * Battery: 3 Minutes
  * Power Adapter: 15 Minutes
  * Show battery status in menu bar
    * Show percentage

### Manual
* Install [homebrew](https://brew.sh/)
  * `brew bundle install`
* Disable Press And Hold
  * `defaults write NSGlobalDomain ApplePressAndHoldEnabled -bool false`
* Symlink VSCode config
  * `sudo ln -s /Users/jiexi/.config/Code/ "/Users/jiexi/Library/Application Support/"`
* Make Fish default shell
  * ```
      sudo bash -c 'echo /usr/local/bin/fish >> /etc/shells'
      chsh -s /usr/local/bin/fish
    ```
  * Restart shell
* Add Day-O to menu bar
  * Disable Icon
  * Enable Startup
  * Format ` E MMM d  h:mm a ` (include surrounding spaces)
  * Disable System Date/Time Widget


### Save Homebrew Packages
`brew bundle dump`
