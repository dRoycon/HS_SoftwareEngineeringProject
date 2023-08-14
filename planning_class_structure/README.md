# The Classes Structure 

``` mermaid
classDiagram
    GraphicalObject <|-- GameObject : Inheritance
    GraphicalObject <|-- TextBox : Inheritance
    GraphicalObject <|-- Joystick : Inheritance

    GameObject <|-- Portal : Inheritance
    GameObject <|-- Box : Inheritance
    GameObject <|-- Entity : Inheritance

    Entity <|-- Enemy : Inheritance
    Entity <|-- Player : Inheritance

    Scene *-- GraphicalObject : Composition
    Scene <|-- GameScene : Inheritance

    Controler *-- Joystick : Composition

    GameplayScreen *-- GameScene : Composition
    GameScreen *-- Controler : Composition

    StartingScreen *-- Scene : Composition

    LevelSelctingScreen *-- Scene : Composition
    SettingsScreen *-- Scene : Composition
    PauseGameplayScreen *-- screen : Composition


```