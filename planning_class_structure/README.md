# The Classes Diagrams Structure 

``` mermaid
classDiagram
    Screen <|-- StartingScreen
    Screen <|-- LevelSelectingScreen
    Screen <|-- SettingsScreen
    Screen <|-- PauseGameplayScreen
    Screen <|-- GameplayScreen

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

    class GraphicalObject{
        +PointF position
        +Size size
        +Color color
        +Bitmap texture
    }

    class GameObject{
        +Update(Position)
    }

    class Scene{
        +List<GraphicalObject> graphicalObjects
    }

    class Scene{
        +List<GameObject> gameObjects
    }

    class TextBox{
        +String message
    }


```