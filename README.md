# Pause_Resume_Menu

## INGREDIENTS
- A "GamePlay" map with a game already functioning
- Create a "MenuWidget" widget blueprint - right click > user interface > WidgetBlueprint
  - Add to it one button for "Play" and another for "Quit"
- Create another level map "Menu"

## PREPARATION
- in project settings > maps and modes, change starting menu to "Menu"

## COOKING

### Main Menu
- in the level BP for the main menu, event graph, onBeginPlay
  - Set input to UI only
  - Show mouse cursor
  - Create menu widget and add it to viewport.
- Add an onClicked event for Play button
  - Set input mode to game only
  - Open gameplay level
  - remove widget
- Add an onClicked event for Quit button
  - Execute console command : "quit"
