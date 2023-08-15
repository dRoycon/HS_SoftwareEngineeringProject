# The Classes Structure 

``` mermaid
classDiagram
    GraphicalObject <|-- GameObject 
    GraphicalObject <|-- TextBox
    GraphicalObject <|-- Joystick

    GameObject <|-- Box
    GameObject <|-- Entity

    Entity <|-- NPC
    Entity <|-- Player

    Scene *-- GraphicalObject
    GameObject <|-- Portal

    Scene <|-- GameScene

    GameScene *-- Player
    GameScene *-- GameObject

    Controler *-- Joystick

    GameplayScreen *-- GameScene
    GameplayScreen *-- Controler

    StartingScreen *-- Scene

    LevelSelctingScreen *-- Scene
    SettingsScreen *-- Scene
    PauseGameplayScreen *-- Scene


```