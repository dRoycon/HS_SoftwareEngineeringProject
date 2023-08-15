# The Classes Diagrams Structure

``` mermaid
classDiagram
    iDrawScreen <|.. StartingScreen
    iDrawScreen <|.. LevelSelectingScreen
    iDrawScreen <|.. SettingsScreen
    iDrawScreen <|.. PauseGameplayScreen
    iDrawScreen <|.. GameplayScreen

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
    GameplayScreen *-- GameScene

    class iDrawScreen{
        <<interface>>
        DrawScreen()
    }

    class GraphicalObject{
        +PointF position
        +Size size
        +Color color
        +Bitmap texture
    }

    class GameObject{
        +Update(PointF position)
    }

    class Scene{
        +List<GraphicalObject> graphicalObjects
    }

    class GameScene{
        +List<GameObject> gameObjects
        +Player player

    }

    class Player{
        +Portal[] portals
    }

    class TextBox{
        +String message
    }


```

#### [Player](planning_class_structure/classes_description/Player.md)<br />
#### [Portal](planning_class_structure/classes_description/Portal.md)<br />
#### [Scene](planning_class_structure/classes_description/Scene.md)<br />