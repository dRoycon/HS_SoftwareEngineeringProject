# The Classes Structure 

``` mermaid
classDiagram
    GraphicalObject <|-- GameObject 
    GraphicalObject <|-- TextBox
    GraphicalObject <|-- Joystick

    GameObject <|-- Portal
    GameObject <|-- Box
    GameObject <|-- Entity

    Entity <|-- NPC
    Entity <|-- Player

    Scene *-- GraphicalObject
    Scene <|-- GameScene

    Player *-- GameScene

    Controler *-- Joystick

    GameplayScreen *-- GameScene
    GameplayScreen *-- Controler

    StartingScreen *-- Scene

    LevelSelctingScreen *-- Scene
    SettingsScreen *-- Scene
    PauseGameplayScreen *-- Seane


```