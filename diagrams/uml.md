# StudyQuest — System UML Diagram

```mermaid
classDiagram
    class User {
        +id: Int
        +email: String
        +passwordHash: String
    }

    class Module {
        +id: Int
        +userId: Int
        +name: String
        +description: String
    }

    class Topic {
        +id: Int
        +moduleId: Int
        +title: String
        +confidence: Int
        +notes: String
    }

    class AIRanking {
        +id: Int
        +topicId: Int
        +difficultyScore: Int
        +timeDemand: Int
        +importance: Int
        +dependencies: String[]
    }

    class Flashcard {
        +id: Int
        +topicId: Int
        +type: String
        +question: String
        +answer: String
        +options: String[]
    }

    class Timetable {
        +id: Int
        +userId: Int
        +topicId: Int
        +date: Date
        +allocatedMinutes: Int
        +status: String
    }

    User "1" --> "many" Module
    Module "1" --> "many" Topic
    Topic "1" --> "1" AIRanking
    Topic "1" --> "many" Flashcard
    User "1" --> "many" Timetable
