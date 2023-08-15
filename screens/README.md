# Screens 

## Screens Layout
``` mermaid
flowchart LR

    id["The SettingScreen can only return to its previous you can *not* do StartingScreen --> SettingScreen --> PauseScreen --> GameplayScreen"]

    StartingScreen --> GameplayScreen
    StartingScreen <--> LevelSelectingScreen
    StartingScreen <--> SettingScreen

    LevelSelectingScreen --> GameplayScreen

    GameplayScreen <--> PauseScreen
    PauseScreen <--> SettingScreen
    PauseScreen --> StartingScreen

```
## Starting Screen


## Settings


## Leves Selecting Screen


## Gameplay Screen


## Pause Screen