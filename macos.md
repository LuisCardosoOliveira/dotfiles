###############################################################################

# General UI/UX

###############################################################################

# Set sidebar icon size to medium

defaults write NSGlobalDomain NSTableViewDefaultSizeMode -int 2

# Automatically quit printer app once the print jobs complete

defaults write com.apple.print.PrintingPrefs "Quit When Finished" -bool true

# Check for software updates daily, not just once per week

defaults write com.apple.SoftwareUpdate ScheduleFrequency -int 1

###############################################################################

# Trackpad, mouse, keyboard, Bluetooth accessories, and input

###############################################################################

# Trackpad: enable tap to click for this user and for the login screen

defaults write com.apple.driver.AppleBluetoothMultitouch.trackpad Clicking -bool true
defaults -currentHost write NSGlobalDomain com.apple.mouse.tapBehavior -int 1
defaults write NSGlobalDomain com.apple.mouse.tapBehavior -int 1

# Trackpad: map bottom right corner to right-click

defaults write com.apple.driver.AppleBluetoothMultitouch.trackpad TrackpadCornerSecondaryClick -int 2
defaults write com.apple.driver.AppleBluetoothMultitouch.trackpad TrackpadRightClick -bool true
defaults -currentHost write NSGlobalDomain com.apple.trackpad.trackpadCornerClickBehavior -int 1
defaults -currentHost write NSGlobalDomain com.apple.trackpad.enableSecondaryClick -bool true

# Disable “natural” (Lion-style) scrolling

defaults write NSGlobalDomain com.apple.swipescrolldirection -bool false

# Increase sound quality for Bluetooth headphones/headsets

defaults write com.apple.BluetoothAudioAgent "Apple Bitpool Min (editable)" -int 40

# Set a blazingly fast keyboard repeat rate

defaults write NSGlobalDomain KeyRepeat -int 2
defaults write NSGlobalDomain InitialKeyRepeat -int 15

###############################################################################

# Screen

###############################################################################

# Save screenshots to the desktop

defaults write com.apple.screencapture location -string "${HOME}/Desktop"

# Save screenshots in PNG format (other options: BMP, GIF, JPG, PDF, TIFF)

defaults write com.apple.screencapture type -string "png"

# Disable shadow in screenshots

defaults write com.apple.screencapture disable-shadow -bool false

###############################################################################

# Finder

###############################################################################

# Finder: show hidden files by default

defaults write com.apple.Finder AppleShowAllFiles -bool true

# When performing a search, search the current folder by default

defaults write com.apple.finder FXDefaultSearchScope -string "SCcf"

# Disable the warning when changing a file extension

defaults write com.apple.finder FXEnableExtensionChangeWarning -bool false

# Avoid creating .DS_Store files on network volumes

defaults write com.apple.desktopservices DSDontWriteNetworkStores -bool true

# Use list view in all Finder windows by default

# Four-letter codes for the other view modes: `icnv`, `clmv`, `Flwv`

defaults write com.apple.finder FXPreferredViewStyle -string "Nlsv"

# Disable the warning before emptying the Trash

defaults write com.apple.finder WarnOnEmptyTrash -bool false

# Empty Trash securely by default

defaults write com.apple.finder EmptyTrashSecurely -bool true

###############################################################################

# Dock, Dashboard, and hot corners

###############################################################################

# Enable highlight hover effect for the grid view of a stack (Dock)

defaults write com.apple.dock mouse-over-hilite-stack -bool true

# Set the icon size of Dock items to 36 pixels

defaults write com.apple.dock tilesize -int 36

# Change minimize/maximize window effect

defaults write com.apple.dock mineffect -string "scale"

# Minimize windows into their application’s icon

defaults write com.apple.dock minimize-to-application -bool false

# Show only open applications in the Dock

defaults write com.apple.dock static-only -bool true

# Don’t automatically rearrange Spaces based on most recent use

defaults write com.apple.dock mru-spaces -bool false

# Remove the auto-hiding Dock delay

defaults write com.apple.dock autohide-delay -float 0

# Remove the animation when hiding/showing the Dock

defaults write com.apple.dock autohide-time-modifier -float 0

###############################################################################

# Mail

###############################################################################

# Display emails in threaded mode, sorted by date (oldest at the top)

defaults write com.apple.mail DraftsViewerAttributes -dict-add "DisplayInThreadedMode" -string "yes"
defaults write com.apple.mail DraftsViewerAttributes -dict-add "SortedDescending" -string "yes"
defaults write com.apple.mail DraftsViewerAttributes -dict-add "SortOrder" -string "received-date"

# Disable inline attachments (just show the icons)

defaults write com.apple.mail DisableInlineAttachmentViewing -bool true
