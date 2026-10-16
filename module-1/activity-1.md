# Activity 1: How the Internet Works
Students simulate the interaction between a browser, server, and database to understand how requests are processed and responses are returned.
# Solution

**Scenario: User Login**

Three students act as the browser, server, and database.

**Step 1: Browser (Frontend)**

* The user enters a username and password.
* The browser sends a login request to the server.

**Step 2: Server (Backend)**

* The server receives the login request.
* It checks the login details against the information stored in the database.

**Step 3: Database**

* The database checks whether the user information matches the stored records.
* It returns the result to the server.

**Step 4: Response**

* If the login details are correct, the server sends a success response.
* If the details are incorrect, the server sends an error response.
* The browser displays the appropriate message to the user.

### Flowchart

```text
       START
         |
         v
  User Enters Login Details
         |
         v
  Browser Sends Request
         |
         v
   Server Receives Request
         |
         v
   Database Checks Details
         |
         v
   Are Details Correct?
       /       \
     Yes        No
      |          |
      v          v
 Login Success  Login Failed
      |          |
      v          v
 Display Result in Browser
         |
         v
        STOP
```

### Result

The activity demonstrates how a browser sends requests to a server, how the server interacts with a database, and how the response is returned to the browser.


