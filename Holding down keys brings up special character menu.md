## Issue
I noticed that when holding down keys on my Mac, instead of repeating the character it would pop open a special character menu. This was especially annoying when trying to navigate around using Vim keybindings.

![[key-repeat-menu.png]]

I couldn't find any simple way to fix this in the settings but discovered a command that turns it off. 
## Solution
Start by heading to `System Preferences > Keyboard` and set your desired Repeat Rate and Delay.
![[system-pref-keyboard.png]]

After that open your terminal and enter this command:
`defaults write -g ApplePressAndHoldEnabled -bool false`

Now you are free to hold keys are have them repeat like they should.