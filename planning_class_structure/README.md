# The Classes Structure 

``` mermaid
classDiagram
    GraphicalObject <|-- TextBox
    GraphicalObject <|-- JoyStick
    GraphicalObject <|-- GameObject

    GameObject <|-- Portal
    GameObject <|-- Box
    GameObject <|-- Entity

    Entity <|-- Enemy
    Entity <|-- Player

    Scene <|-- GameScene

    GameScreen
```