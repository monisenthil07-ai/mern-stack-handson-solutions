# Activity 3: Real-world Scenario Mapping Students identify common applications they use daily and map their frontend, backend, and database components.
# Activity 3: Real-World Scenario Mapping

**Aim:** To identify commonly used applications and understand their frontend, backend, and database components.

### 1. Introduction

Real-world applications use three main components: frontend, backend, and database. These components work together to provide services to users.

### 2. Example 1: Instagram

| Component | Description                                                  | Example Technologies |
| --------- | ------------------------------------------------------------ | -------------------- |
| Frontend  | Displays posts, profiles, images, and buttons to users.      | HTML, CSS, React     |
| Backend   | Handles login, likes, comments, and messages.                | Python, Node.js      |
| Database  | Stores user details, posts, comments, and other information. | PostgreSQL, MySQL    |

**Working:** When a user likes a post, the frontend sends a request to the backend. The backend updates the information in the database and sends a response to the frontend.

### 3. Example 2: Online Shopping Application

| Component | Description                                               | Example Technologies  |
| --------- | --------------------------------------------------------- | --------------------- |
| Frontend  | Displays products, prices, and shopping cart details.     | HTML, CSS, JavaScript |
| Backend   | Processes orders, payments, and customer requests.        | Java, Node.js         |
| Database  | Stores product details, customer information, and orders. | MySQL, MongoDB        |

**Working:** When a customer purchases a product, the frontend sends the order details to the backend. The backend processes the order and stores the relevant information in the database.

### 4. Example 3: WhatsApp

| Component | Description                                               | Example Technologies                     |
| --------- | --------------------------------------------------------- | ---------------------------------------- |
| Frontend  | Displays chats, contacts, and messages.                   | React Native, native mobile technologies |
| Backend   | Handles message delivery and communication between users. | Server-side technologies                 |
| Database  | Stores relevant account information and message data.     | Database and storage systems             |

**Working:** When a user sends a message, the application sends it through the backend infrastructure to the recipient. The application uses storage systems to manage relevant data.

### 5. Architecture Diagram

```text
          USER
            |
            v
   +------------------+
   |     FRONTEND     |
   |  User Interface  |
   +------------------+
            |
            v
   +------------------+
   |      BACKEND     |
   | Business Logic   |
   +------------------+
            |
            v
   +------------------+
   |     DATABASE     |
   |   Stores Data    |
   +------------------+
            |
            v
     Backend Response
            |
            v
   Frontend Displays
       the Result
```

### 6. Advantages

1. **Frontend:** Provides a user-friendly interface.
2. **Backend:** Processes requests and applies business rules.
3. **Database:** Stores and manages application data.
4. **Integration:** Allows the components to work together efficiently.
5. **Scalability:** Enables applications to support growing numbers of users.

### Result

The frontend, backend, and database components of commonly used applications were identified and mapped. This activity helped explain how these components work together to build and operate real-world applications.
