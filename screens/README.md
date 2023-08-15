# Screens 

## Screens Layout
``` mermaid
stateDiagram-v2

    StartingScreen --> GameplayScreen
    GameplayScreen --> StartingScreen

    GameplayScreen --> PauseScreen
    PauseScreen --> GameplayScreen

    state  "SettingScreen can only rerurn to the previous screen" as s1

    PauseScreen --> StartingScreen
    PauseScreen --> SettingScreen
    SettingScreen --> PauseScreen

    LevelSelectingScreen --> GameplayScreen
    StartingScreen --> LevelSelectingScreen
    LevelSelectingScreen --> StartingScreen
    LevelSelectingScreen --> GameplayScreen
    StartingScreen --> LevelSelectingScreen

    StartingScreen --> SettingScreen
    SettingScrenn --> StartingScreen

```
## Starting Screen


## Settings


## Leves Selecting Screen


## Gameplay Screen


## Pause Screen