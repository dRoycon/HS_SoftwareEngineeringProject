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

*Note: The SettingScreen can only return to its previous you can **not** do ```StartingScreen --> SettingScreen --> PauseScreen --> GameplayScreen```

## Sketches

### Starting Screen

### Settings

### Leves Selecting Screen

### Gameplay Screen

### Pause Screen
