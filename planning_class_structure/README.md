# The Classes Structure 

``` mermaid
classDiagram
    GameScene *-- GameObject
    GraphicalObject <|-- Joystick

    GraphicalObject <|-- GameObject 
    GraphicalObject <|-- TextBox

    GameObject <|-- Box
    GameObject <|-- Entity

    Entity <|-- NPC
    Entity <|-- Player

    Scene <|-- GameScene

    Scene *-- GraphicalObject
    GameObject <|-- Portal


    GameScene *-- Player

    Controler *-- Joystick

    GameplayScreen *-- GameScene
    GameplayScreen *-- Controler

    StartingScreen *-- Scene

    LevelSelctingScreen *-- Scene
    SettingsScreen *-- Scene
    PauseGameplayScreen *-- Scene


```