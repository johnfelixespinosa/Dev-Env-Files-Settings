# Mac Settings

## Create and direct screenshots to Screenshots dir
```
mkdir ~/Desktop/Screenshots
defaults write com.apple.screencapture location ~/Desktop/Screenshots
```

## Fixes font smoothing issue
```
defaults write -g CGFontRenderingFontSmoothingDisabled -bool FALSE
```
![font smoothing gif](/img/font_smoothing.gif)

## Increase sound quality for bluetooth/wireless headsets
```
defaults write com.apple.BluetoothAudioAgent "Apple Bitpool Min (editable)" -int 40
```

## Disable press-and-hold for keys in favor of key repeat
```
defaults write NSGlobalDomain ApplePressAndHoldEnabled -bool false
```

## Set a blazingly fast keyboard repeat rate
```
defaults write NSGlobalDomain KeyRepeat -int 1
defaults write NSGlobalDomain InitialKeyRepeat -int 15
```

## Require password immediately after sleep or screen saver begins
```
defaults write com.apple.screensaver askForPassword -int 1
defaults write com.apple.screensaver askForPasswordDelay -int 0
```

## Finder: show hidden files by default
```
defaults write com.apple.finder AppleShowAllFiles -bool true
```

## Finder: show all filename extensions
```
defaults write NSGlobalDomain AppleShowAllExtensions -bool true
```

## Privacy: don’t send search queries to Apple
```
defaults write com.apple.Safari UniversalSearchEnabled -bool false
defaults write com.apple.Safari SuppressSearchSuggestions -bool true
```