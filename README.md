# Santander-dev-week-2024

Java RESTful API criada para a Santander Dev Week.

# Class Diagram

```mermaid
classDiagram
    class User {
        - String name
        - Account account
        - Feature[] features
        - Card card
        - News[] news
    }
    
    class Account {
        - String number
        - String agency
        - number balance
        - number limit
    }
    
    class Feature {
        - String icon
        - String description
    }

    class Card {
        - String number
        - number limit
    }
    
    class News {
        - String icon
        - String description
    }
    
    User *-- Account
    User *-- Feature
    User *-- Card
    User *-- News
