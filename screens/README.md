# Screens 

## Screens Layout
``` mermaid
stateDiagram-v2

    StartingScreen --> GameplayScreen
    GameplayScreen --> StartingScreen

    GameplayScreen --> PauseScreen
    PauseScreen --> GameplayScreen

    PauseScreen --> StartingScreen
    PauseScreen --> SettingScreen
    SettingScreen --> PauseScreen

    StartingScreen --> LevelSlectingScreen
    LevelSlectingScreen --> StartingScreen
    LevelSelectingScreen --> GameplayScreen
```
## Starting Screen


## Settings


## Leves Selecting Screen


## Gameplay Screen


## Pause Screen