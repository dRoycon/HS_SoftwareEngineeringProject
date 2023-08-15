# The Classes Structure 

``` mermaid
classDiagram

    StartingScreen *-- Scene
    LevelSelectingScreen *-- Scene
    SettingsScreen *-- Scene
    PauseGameplayScreen *-- Scene

    Scene *-- GraphicalObject
    Scene <|-- GameScene 

    GraphicalObject <|-- TextBox
    GraphicalObject <|-- GameObject

    GameObject <|-- Box
    GameObject <|-- Entity
    GameplayScreen *-- GameObject 

    Entity <|-- NPC
    Entity <|-- Player
```