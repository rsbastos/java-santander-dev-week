# Java API RESTful with Deploy on Railway - (DIO- Bootcamp Santander Fullstack Java  + Angular) 

## Main Technologies
- **Java 17**
- **Spring Boot 3**
- **Spring Data JPA**
- **OpenAPI (Swagger)**
- **Railway**

## Class Diagram

```mermaid
classDiagram
  class User {
    -name: String
    -account: Account
    -features: Feature[]
    -card: Card
    -news: News[]
  }

  class Account {
    -number: String
    -agency: String
    -balance: number
    -limit: number
  }

  class Feature {
    -icon: String
    -description: String
  }

  class Card {
    -number: String
    -limit: number
  }

  class News {
    -icon: String
    -description: String
  }

  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1" Card
  User "1" *-- "N" News
```
