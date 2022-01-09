# printdialog

Print dialog. Bash and Zenity.

In my particular use case (linux desktop, Kyocera copier) I find the application print dialogs super-inconsistent. They don't seem to have been written/tested with the various features (folding, stapling, different sizes of paper) of a copier in mind. But printing from the command-line tends to be understandable and consistent. This is my own print dialog to avoid having to remember arcane `lp` arguments that pertain to my particular printer.

Zenity is kind of fun: easy, quick results.

## Good Intentions (and perhaps some ill-advised ones as well!)
- TODO: won't print multiple copies (to my Brother printer)
- TODO: check return codes from dialogs and leave values unchanged when "cancel"
- DONE: optionally accept filename(s) as arguments to script
- DONE: optionally accept printer name as argument to script
- DONE: skip initial prompts for arguments provided
- TODO: fill out wip features
- TODO: Utilities: e.g., round out a pdf to have a number of pages divisible by 4 (matching page size)
- TODO: Presets / Utilities / Other offer numerals in first column for easy keyboard access?

## Notes
https://github.com/dylanaraps/pure-bash-bible#arrays
https://help.gnome.org/users/zenity/stable/
https://www.cups.org/doc/options.html
Print from bypass tray: -o InputSlot=MF1
lpstat -v
lpoptions -p "StT-Kyocera-TASKalfa-2552ci-(KPDL)" -l
lpadmin -p ... -o ....
