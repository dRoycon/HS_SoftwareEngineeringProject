# The Classes Structure 

``` mermaid
classDiagram
    GraphicalObject <|-- GameObject
    GraphicalObject <|-- TextBox
    GraphicalObject <|-- Joystick

    GameObject <|-- Portal
    GameObject <|-- Box
    GameObject <|-- Entity

    Entity <|-- Enemy
    Entity <|-- Player

    Scene *-- GraphicalObject
    Scene <|-- GameScene

    Controler *-- Joystick

    GameplayScreen *-- GameScene
    GameScreen *-- Controler

    StartingScreen *-- Scene

    LevelSelctingScreen *-- Scene
    SettingsScreen *-- Scene
    PauseGameplayScreen *-- screen


```