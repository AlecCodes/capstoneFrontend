# Blood Glucose Diary for Diabetics
-----

## Overview
A CRUD app for diabetics to help them track their daily carbohydrate intake. Foods and their associated carb value can be entered into the App by users, and the app will store the data and tell them their average daily carbohydrate intake, and whether their daily intake falls below or above the threshold. 

-----
## Tech Stack
| Component | Tech Used |
|-------------------|-------------|
| Backend Framework | Spring Boot |
| Database | postgresSQL |
| Deployment        | Heroku      |  
| Frontend          | React       |  
| Styling           | Bootstrap   |

-----
## Backend
- Spring Boot CRUD app
- Deployment using Heroku CLI tool
- Date stored as a string, which is parsed by frontend 

### Data model
| Property | Type   |
|----------|--------|
| id     | int |
| Date     | String |
| Carbs    | int    |
| Name     | String |

### Routes
| HTTP Method  | Action                | url route |
|--------------|-----------------------|-----------|
| GET          | Display Index of Days | "/"       |
| POST         | New Food              | "/"       |
| DELETE       | Destroy               | "/{id}"   |
| PUT          | Update Food           | "/{id}"   |
| GET          | Display Food          | "/{id}"   |

-----
## Frontend
- Main index page displays days
- Day inde page filters out only results for that day from data loader
- Edit, Delete functions on Food show page

### Routes
| Route          | Content                   |
|----------------|---------------------------|
| "/"            | Display list of days      |
| "dayshow/:day" | Show day's index of foods |
| "show/:id"     | Show food info            |
| "edit/:id"     | Edit food                 |
| "create"       | Create food               |

## Wireframe

https://i.imgur.com/ctVm120.png