# Activity 1: Responsive Layout Design
Students build a responsive landing page that adapts to desktop, tablet, and mobile devices.
## Activity 1: Responsive Layout Design – Solution

### 1. Aim

To design and develop a responsive landing page using HTML and CSS that automatically adjusts its layout for desktop, tablet, and mobile devices.

### 2. Technologies Used

* **HTML:** Creates the structure of the webpage.
* **CSS:** Styles the webpage and makes it responsive.
* **Media Queries:** Adjust the layout according to screen size.

### 3. Program

Create a file named `index.html` and add the following code.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Landing Page</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
        }

        header {
            background-color: #2563eb;
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav {
            background-color: #1e40af;
            padding: 12px;
            text-align: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 15px;
        }

        .hero {
            background-color: #eff6ff;
            text-align: center;
            padding: 60px 20px;
        }

        .hero h2 {
            font-size: 36px;
            margin-bottom: 15px;
        }

        .hero p {
            margin-bottom: 20px;
        }

        button {
            background-color: #2563eb;
            color: white;
            padding: 12px 25px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .features {
            display: flex;
            justify-content: center;
            gap: 20px;
            padding: 30px;
        }

        .card {
            background-color: #f3f4f6;
            padding: 25px;
            text-align: center;
            flex: 1;
            border-radius: 8px;
        }

        footer {
            background-color: #1e3a8a;
            color: white;
            text-align: center;
            padding: 15px;
        }

        /* Tablet Layout */
        @media (max-width: 768px) {
            .features {
                flex-wrap: wrap;
            }

            .card {
                flex: 1 1 40%;
            }

            .hero h2 {
                font-size: 28px;
            }
        }

        /* Mobile Layout */
        @media (max-width: 480px) {
            nav a {
                display: block;
                margin: 8px;
            }

            .features {
                flex-direction: column;
            }

            .card {
                width: 100%;
            }

            .hero h2 {
                font-size: 24px;
            }

            .hero {
                padding: 35px 15px;
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>My Responsive Website</h1>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#features">Features</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>

    <section class="hero" id="home">
        <h2>Welcome to Our Website</h2>
        <p>Learn, explore, and grow with our responsive web design.</p>
        <button onclick="alert('Welcome to our website!')">
            Get Started
        </button>
    </section>

    <section class="features" id="features">
        <div class="card">
            <h3>Easy to Use</h3>
            <p>A simple and user-friendly design.</p>
        </div>

        <div class="card">
            <h3>Responsive Design</h3>
            <p>Works on desktops, tablets, and mobiles.</p>
        </div>

        <div class="card">
            <h3>Modern Layout</h3>
            <p>A clean and attractive webpage.</p>
        </div>
    </section>

    <footer id="contact">
        <p>&copy; 2026 My Responsive Website</p>
    </footer>

</body>
</html>
```

### 4. Procedure

1. Open Visual Studio Code.
2. Create a folder named `responsive-landing-page`.
3. Create an `index.html` file inside the folder.
4. Copy and paste the above code.
5. Save the file.
6. Open `index.html` in a browser.
7. Resize the browser window to test the responsive layout.

### 5. Responsive Design

| Device  | Screen Width   | Layout                                                       |
| ------- | -------------- | ------------------------------------------------------------ |
| Desktop | Above 768px    | Feature cards appear in a row.                               |
| Tablet  | 481px–768px    | Feature cards wrap into multiple rows.                       |
| Mobile  | 480px or below | Feature cards appear vertically, and navigation links stack. |

### 6. Expected Output

The landing page displays:

* A website header.
* Navigation links.
* A welcome section with a **Get Started** button.
* Three feature cards.
* A footer.

The layout automatically adjusts to different screen sizes.

### 7. Result

Thus, a responsive landing page was successfully developed using HTML, CSS Flexbox, and CSS Media Queries. The webpage adapts to desktop, tablet, and mobile devices.
