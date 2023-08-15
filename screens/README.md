# Screens 

## Screens Layout
``` mermaid
flowchart LR

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