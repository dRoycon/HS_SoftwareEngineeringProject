# The Classes Structure 

``` mermaid
classDiagram
    Screen <|-- StartingScreen
    Screen <|-- LevelSelectingScreen
    Screen <|-- SettingsScreen
    Screen <|-- PauseGameplayScreen

    StartingScreen *-- Scene
    LevelSelectingScreen *-- Scene
    SettingsScreen *-- Scene
    PauseGameplayScreen *-- Scene

    Scene *-- GraphicalObject
    Scene <|-- GameScene 

    GraphicalObject <|-- Joystick
    GraphicalObject <|-- TextBox
    GraphicalObject <|-- GameObject

    GameObject <|-- Portal
    GameObject <|-- Box
    GameObject <|-- Entity
    GameScene *-- GameObject 


    Entity <|-- Player
    Entity <|-- NPC

    NPC <|-- Enemy

    GameplayScreen *-- GameScene
    GameplayScreen *-- NPC
    GameplayScreen *-- Player
```