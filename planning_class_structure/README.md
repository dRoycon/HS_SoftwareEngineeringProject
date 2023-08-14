# The Classes Structure 

``` mermaid
classDiagram
    GraphicalObject <|-- TextBox
    GraphicalObject <|-- Joystick
    GraphicalObject <|-- GameObject

    GameObject <|-- Portal
    GameObject <|-- Box
    GameObject <|-- Entity

    Entity <|-- Enemy
    Entity <|-- Player

    Scene *-- GraphicalObject
    Scene <|-- GameScene

    Controler *-- Joystick

    GameScreen *-- GameScene
    GameScreen *-- Controler

    StartingScreen *-- Scene

```