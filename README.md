# Flashcards

A simple and quick recipe for flashcard-like learning on Mac OS.

## Setup

1. Create a folder, e.g. _~/Flashcards_
2. Open Automator.app
3. Create a new Automator application; save as _~/Applications/Flashcards.app_

### Configure Automator App

1. Choose _Get Specified Finder Items_
2. Select the folder created above.
3. Choose _Open Finder Items_
4. Ensure that _Open with:_ is set to _Default Application_
5. Choose _Set Folder Views_
6. Change to _Gallery View_
7. Check _Apply window properties_
8. Uncheck all options
9. Save the Automator app
10. Add an icon to the app
11. Create an alias to the app and save to _~/Desktop_
12. Add the icon to the alias

### Configure cron

1. In terminal `crontab -e`
2. Add a line indicating when you want to be prompted to study, e.g.

	`0 12 18 * * * open ~/Applications/Flashcards.app`

1. Given the example, your Flashcards folder will open at noon and 6pm every day.  The position of the folder will be that same as when you last viewed it, except that fullscreen doesn't seem to be remembered as of this writing.		
	
## How to Use

1. Drop screenshots of things you want to learn into _~/Flashcards_
3. Manage the items in _~/Flashcards_ as you see fit, e.g., delete them when you have learned them.
4. When prompted spend as much time as you want, review items, then close the folder when done.
5. To study on demand, click the alias on the desktop.
