# General Setup Instructions

## Custom Keyboard Mappings File
1. Edit keymap file (found in tmk_keyboard-master --> keyboard --> respective keyboard layout folder) or create a new one
2. Delete any folders (.dep, gh60 folders)
3. Run `make KEYMAP=<name>` where the keymap file is `keymap_<name>.c`
   - may need to install dfu-programmer (`sudo apt-get update; sudo apt-get install dfu-programmer`)
   - may need to install avr-gcc (`sudo apt-get update; sudo apt-get install gcc-avr binutils-avr avr-libc`)

## Flashing Custom Firmware
**Note**: May need to run `zadig.exe` in `windows/tools` sometime during the below steps.

1. In tkg-toolkit-master, under windows run `setup.bat`
   - choose RevCHN
   - choose default
   - choose lufa
2. Drag the `.hex` file generated from step 2 onto `reflash.bat`

Voila, your keyboard should be flashed with your new mappings! 
