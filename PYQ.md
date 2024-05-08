## Simple Navigation Bar

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Navigation Bar</title>
  <style>
    /* Style for the navigation bar */
    .navbar {
      background-color: #333;
      overflow: hidden;
    }

    /* Style for the links inside the navigation bar */
    .navbar a {
      float: left;
      display: block;
      color: white;
      text-align: center;
      padding: 14px 20px;
      text-decoration: none;
    }

    /* Change color on hover */
    .navbar a:hover {
      background-color: #ddd;
      color: black;
    }
  </style>
</head>
<body>

<div class="navbar">
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#services">Services</a>
  <a href="#contact">Contact</a>
</div>

<div style="padding: 20px;">
  <!-- Content goes here -->
  <h2>Simple Navigation Bar Example</h2>
  <p>This is a simple example of a navigation bar using HTML and CSS.</p>
</div>

</body>
</html>
```

<hr>

## Events in HTML 

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Events Example</title>
  <script>
    // Function to handle button click event
    function handleClick() {
      alert("Button clicked!");
    }

    // Function to handle input change event
    function handleChange() {
      var inputValue = document.getElementById("textInput").value;
      alert("Input changed. New value: " + inputValue);
    }

    // Function to handle mouse over event
    function handleMouseOver() {
      document.getElementById("mouseOverDiv").innerHTML = "Mouse Over Event Occurred!";
    }

    // Function to handle mouse out event
    function handleMouseOut() {
      document.getElementById("mouseOverDiv").innerHTML = "";
    }
  </script>
</head>
<body>
  <h2>Events Example</h2>
  
  <!-- Button with click event -->
  <button onclick="handleClick()">Click Me</button>
  <br><br>

  <!-- Input field with change event -->
  <label for="textInput">Enter Text:</label>
  <input type="text" id="textInput" onchange="handleChange()">
  <br><br>

  <!-- Div with mouse over and mouse out events -->
  <div id="mouseOverDiv" onmouseover="handleMouseOver()" onmouseout="handleMouseOut()" style="border: 1px solid black; width: 200px; height: 100px;"></div>
</body>
</html>
```

<hr>

### Question 1) A. Indicate the loading state of a component or page with bootstrap spinners, built entirely with HTML, CSS.
### B. Convert any Javascript value to a JSON string 

**Question 1A: Indicate the loading state of a component or page with Bootstrap spinners**

```html
<!-- HTML code to display a Bootstrap spinner while loading -->
<div class="text-center">
  <div class="spinner-border" role="status">
    <span class="visually-hidden">Loading...</span>
  </div>
  <p>Loading...</p>
</div>
```

**Question 1B: Convert any JavaScript value to a JSON string**

```javascript
// JavaScript code to convert a JavaScript value to a JSON string
const data = { 
  name: "John", 
  age: 30, 
  city: "New York" 
};

const jsonString = JSON.stringify(data);
console.log(jsonString);
```

<hr>

### 2A. Using Grid System demonstrate row with three columns divided unevenly, Row with three columns divided evenly. 
### 2B. Create CV using HTML, CSS.

**Question 2A: Using Grid System demonstrate row with three columns divided unevenly, Row with three columns divided evenly.**

```html
<!-- HTML code to demonstrate rows with three columns divided unevenly and evenly using Bootstrap Grid System -->
<div class="container">
  <!-- Row with three columns divided unevenly -->
  <div class="row">
    <div class="col-md-4">Column 1</div>
    <div class="col-md-3">Column 2</div>
    <div class="col-md-5">Column 3</div>
  </div>
  <!-- Row with three columns divided evenly -->
  <div class="row">
    <div class="col">Column 1</div>
    <div class="col">Column 2</div>
    <div class="col">Column 3</div>
  </div>
</div>
```

**Question 2B: Create CV using HTML, CSS.**

```html
<!-- HTML code to create a basic CV using HTML and CSS -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My CV</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 800px;
      margin: 20px auto;
      padding: 20px;
      border: 1px solid #ccc;
    }
    h1, h2, h3 {
      margin-bottom: 10px;
    }
    p {
      margin: 0;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>John Doe</h1>
    <p>Email: john@example.com</p>
    <p>Phone: 123-456-7890</p>
    <hr>
    <h2>Education</h2>
    <p>Bachelor of Science in Computer Science, University of Example (2010-2014)</p>
    <hr>
    <h2>Experience</h2>
    <h3>Software Developer, ABC Company (2015-2020)</h3>
    <p>Responsible for developing and maintaining web applications using HTML, CSS, and JavaScript.</p>
    <h3>Senior Developer, XYZ Corporation (2020-present)</h3>
    <p>Leading a team of developers in building scalable and efficient software solutions.</p>
    <hr>
    <h2>Skills</h2>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
      <li>Bootstrap</li>
      <li>Angular</li>
      <li>React</li>
    </ul>
  </div>
</body>
</html>
```

<hr>

### 3A. Demonstrate linked contextual classes using list in Bootstrap.
### 3B. Create simple form in HTML and CSS and demonstrate the use of various form elements like inputbox, textbox, submit, and radio button.

**Question 3A: Demonstrate linked contextual classes using lists in Bootstrap.**

```html
<!-- HTML code to demonstrate linked contextual classes using lists in Bootstrap -->
<div class="container">
  <h2>Linked Contextual Classes using Lists</h2>
  <ul class="list-group">
    <li class="list-group-item list-group-item-primary">Primary item</li>
    <li class="list-group-item list-group-item-secondary">Secondary item</li>
    <li class="list-group-item list-group-item-success">Success item</li>
    <li class="list-group-item list-group-item-danger">Danger item</li>
    <li class="list-group-item list-group-item-warning">Warning item</li>
    <li class="list-group-item list-group-item-info">Info item</li>
    <li class="list-group-item list-group-item-light">Light item</li>
    <li class="list-group-item list-group-item-dark">Dark item</li>
  </ul>
</div>
```

**Question 3B: Create a simple form in HTML and CSS and demonstrate the use of various form elements like inputbox, textbox, submit, and radio button.**

```html
<!-- HTML code to create a simple form and demonstrate the use of various form elements -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 400px;
      margin: 20px auto;
      padding: 20px;
      border: 1px solid #ccc;
    }
    label {
      display: block;
      margin-bottom: 5px;
    }
    input[type="text"], input[type="email"], textarea {
      width: 100%;
      padding: 8px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 4px;
      box-sizing: border-box;
    }
    input[type="submit"] {
      background-color: #007bff;
      color: #fff;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      border-radius: 4px;
    }
    input[type="submit"]:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Simple Form</h2>
    <form>
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" placeholder="Enter your name" required>
      
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" placeholder="Enter your email" required>
      
      <label for="message">Message:</label>
      <textarea id="message" name="message" rows="4" placeholder="Enter your message" required></textarea>
      
      <label>Gender:</label>
      <label><input type="radio" name="gender" value="male"> Male</label>
      <label><input type="radio" name="gender" value="female"> Female</label>
      
      <input type="submit" value="Submit">
    </form>
  </div>
</body>
</html>
```

<hr>

### 4A. Write a javascript to validate the following fields of the registration page. 
### i. first name (Name should contain alphabet and length must not be more than 6 characters)
### ii. Password (Password should not be less than 6 character length)
### iii. Email id(must follow pattern name@domain.com)
### iv. Mobile Number (must be of 10 digits)
### v. Address (Must not be empty)
### 4B. Create a dropdown button and split button dropdown using bootstrap.


**Question 4A: JavaScript to validate registration page fields**

```html
<!-- HTML code for registration page -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Registration Page</title>
  <script>
    function validateForm() {
      var firstName = document.getElementById("firstName").value;
      var password = document.getElementById("password").value;
      var email = document.getElementById("email").value;
      var mobile = document.getElementById("mobile").value;
      var address = document.getElementById("address").value;

      if (!/^[a-zA-Z]+$/.test(firstName) || firstName.length > 6) {
        alert("First name should contain only alphabets and length must not be more than 6 characters");
        return false;
      }
      
      if (password.length < 6) {
        alert("Password should be at least 6 characters long");
        return false;
      }
      
      if (!/^[\w-]+(\.[\w-]+)*@([\w-]+\.)+[a-zA-Z]{2,7}$/.test(email)) {
        alert("Please enter a valid email address");
        return false;
      }
      
      if (!/^\d{10}$/.test(mobile)) {
        alert("Mobile number must be of 10 digits");
        return false;
      }
      
      if (address.trim() === "") {
        alert("Address cannot be empty");
        return false;
      }

      return true;
    }
  </script>
</head>
<body>
  <h2>Registration Form</h2>
  <form onsubmit="return validateForm()">
    <label for="firstName">First Name:</label>
    <input type="text" id="firstName" name="firstName" required><br><br>
    
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required><br><br>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required><br><br>
    
    <label for="mobile">Mobile Number:</label>
    <input type="text" id="mobile" name="mobile" required><br><br>
    
    <label for="address">Address:</label>
    <textarea id="address" name="address" rows="4" required></textarea><br><br>
    
    <input type="submit" value="Register">
  </form>
</body>
</html>
```

**Question 4B: Create a dropdown button and split button dropdown using Bootstrap**

```html
<!-- HTML code to create dropdown button and split button dropdown using Bootstrap -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dropdown Buttons</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<body>
  <div class="container">
    <h2>Dropdown Button</h2>
    <div class="btn-group">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        Dropdown Button
      </button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Action</a>
        <a class="dropdown-item" href="#">Another action</a>
        <a class="dropdown-item" href="#">Something else here</a>
      </div>
    </div>
    <br><br>
    <h2>Split Button Dropdown</h2>
    <div class="btn-group">
      <button type="button" class="btn btn-secondary">
        Split Button
      </button>
      <button type="button" class="btn btn-secondary dropdown-toggle dropdown-toggle-split" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        <span class="sr-only">Toggle Dropdown</span>
      </button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Action</a>
        <a class="dropdown-item" href="#">Another action</a>
        <a class="dropdown-item" href="#">Something else here</a>
      </div>
    </div>
  </div>
  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
```

<hr>

### 5A. Design a web page required for an online book store web site. 
### i. Home page : must have 3 frames. 
### ii. Login Page
### iii. Registration Page

# 5B. Create a service named as newservice and demonstrate dependencies injection at component level.


**Question 5A: Design a web page required for an online book store website**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Online Book Store</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    header, footer {
      background-color: #007bff;
      color: #fff;
      text-align: center;
      padding: 10px;
    }
    nav {
      background-color: #f0f0f0;
      padding: 10px;
      text-align: center;
    }
    section {
      display: flex;
      justify-content: space-between;
      margin: 20px;
    }
    article {
      flex: 1;
      margin: 0 10px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Online Book Store</h1>
  </header>
  <nav>
    <a href="#">Home</a> |
    <a href="#">Login</a> |
    <a href="#">Registration</a>
  </nav>
  <section>
    <article>
      <h2>Frame 1</h2>
      <p>Content for Frame 1</p>
    </article>
    <article>
      <h2>Frame 2</h2>
      <p>Content for Frame 2</p>
    </article>
    <article>
      <h2>Frame 3</h2>
      <p>Content for Frame 3</p>
    </article>
  </section>
  <footer>
    <p>&copy; 2024 Online Book Store. All rights reserved.</p>
  </footer>
</body>
</html>
```

**Question 5B: Create a service named as newservice and demonstrate dependencies injection at component level**

```javascript
// JavaScript code for creating a service named "newservice" and demonstrating dependency injection at the component level
import { Injectable } from '@angular/core';

@Injectable({
  providedIn: 'root'
})
export class NewService {
  constructor() { }

  // Method to display a message
  showMessage() {
    console.log('This is a message from the NewService.');
  }
}
```

In the component where you want to inject this service:

```javascript
import { Component, OnInit } from '@angular/core';
import { NewService } from './new.service';

@Component({
  selector: 'app-example',
  templateUrl: './example.component.html',
  styleUrls: ['./example.component.css']
})
export class ExampleComponent implements OnInit {

  constructor(private newservice: NewService) { }

  ngOnInit(): void {
    this.newservice.showMessage(); // Using the service method
  }

}
```

<hr>

### 6A. Add and link Home, About us pages to your App using angular. 
### 6B. Develop and demonstrate the usage of inline, internal and external style sheet using Css.


**Question 6A: Add and link Home, About us pages to your App using Angular**

```bash
ng generate component home
ng generate component about-us
```

Then, you can define the routes in your Angular application:

```javascript
// app-routing.module.ts
import { NgModule } from '@angular/core';
import { Routes, RouterModule } from '@angular/router';
import { HomeComponent } from './home/home.component';
import { AboutUsComponent } from './about-us/about-us.component';

const routes: Routes = [
  { path: '', component: HomeComponent },
  { path: 'home', component: HomeComponent },
  { path: 'about-us', component: AboutUsComponent },
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }
```

Next, create links to navigate between these pages in your HTML template:

```html
<!-- app.component.html -->
<nav>
  <a routerLink="/home" routerLinkActive="active">Home</a>
  <a routerLink="/about-us" routerLinkActive="active">About Us</a>
</nav>
<router-outlet></router-outlet>
```

**Question 6B: Develop and demonstrate the usage of inline, internal, and external style sheets using CSS**

```html
<!-- HTML code with inline, internal, and external style sheets -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Styling Example</title>
  <!-- External style sheet -->
  <link rel="stylesheet" href="styles.css">
  <style>
    /* Internal style sheet */
    body {
      background-color: lightblue;
    }
    h1 {
      color: green;
    }
  </style>
</head>
<body>
  <h1>Inline Style</h1>
  <p>This text is styled using inline CSS.</p>
  <p class="internal">This text is styled using internal CSS.</p>
  <p class="external">This text is styled using external CSS.</p>
</body>
</html>
```

```css
/* styles.css (External style sheet) */
.external {
  color: blue;
}
```

<hr>

### 7A. Develop and Demonstrate Javscript with POP UP boxes and functions for the following problems.
### i. INPUT :  Click on Display Date button using OnClick() function. 
###   OUTPUT : Display Date in the textbox.
### ii. INPUT : A number  n obtained using prompt.
###    OUTPUT : Factorial of n number using alert.

### 7B. Create 5 button with style primary, secondary, success, danger, info using bootstrap

**Question 7A: Develop and Demonstrate JavaScript with POP UP boxes and functions**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>JavaScript Popup Boxes and Functions</title>
  <script>
    // Function to display current date in a textbox
    function displayDate() {
      var currentDate = new Date().toDateString();
      document.getElementById("dateInput").value = currentDate;
    }

    // Function to calculate factorial of a number and display using alert
    function calculateFactorial() {
      var number = prompt("Enter a number:");
      if (number !== null) {
        number = parseInt(number);
        if (number >= 0) {
          var factorial = 1;
          for (var i = 2; i <= number; i++) {
            factorial *= i;
          }
          alert("Factorial of " + number + " is: " + factorial);
        } else {
          alert("Please enter a non-negative integer.");
        }
      }
    }
  </script>
</head>
<body>
  <h2>JavaScript Popup Boxes and Functions</h2>
  <button onclick="displayDate()">Display Date</button>
  <input type="text" id="dateInput">
  <br><br>
  <button onclick="calculateFactorial()">Calculate Factorial</button>
</body>
</html>
```

**Question 7B: Create 5 buttons with style primary, secondary, success, danger, info using Bootstrap**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bootstrap Buttons</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<body>
  <h2>Bootstrap Buttons</h2>
  <button class="btn btn-primary">Primary Button</button>
  <button class="btn btn-secondary">Secondary Button</button>
  <button class="btn btn-success">Success Button</button>
  <button class="btn btn-danger">Danger Button</button>
  <button class="btn btn-info">Info Button</button>
</body>
</html>
```

<hr>

### 8A. Create a webpage that contains a selection box with a list of 5 countries. When the user selects a country, its capital should be printed next in the list. Add Css to customize the properties of font of the capital (color, bold and font size)

### 8B. Convert text '{"name" : "John", "age": 20, "city": "New York"}' into a JavaScript object  and display the result on webpage

**Question 8A: Create a webpage with a selection box to display the capital of a selected country**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Country Capitals</title>
  <style>
    body {
      font-family: Arial, sans-serif;
    }
    #capital {
      color: blue;
      font-weight: bold;
      font-size: 20px;
    }
  </style>
</head>
<body>
  <h2>Country Capitals</h2>
  <select id="country" onchange="displayCapital()">
    <option value="none">Select a country</option>
    <option value="usa">USA</option>
    <option value="uk">UK</option>
    <option value="france">France</option>
    <option value="germany">Germany</option>
    <option value="japan">Japan</option>
  </select>
  <p>Capital: <span id="capital"></span></p>
  <script>
    function displayCapital() {
      var selectBox = document.getElementById("country");
      var capitalSpan = document.getElementById("capital");
      var country = selectBox.value;
      switch (country) {
        case "usa":
          capitalSpan.textContent = "Washington D.C.";
          break;
        case "uk":
          capitalSpan.textContent = "London";
          break;
        case "france":
          capitalSpan.textContent = "Paris";
          break;
        case "germany":
          capitalSpan.textContent = "Berlin";
          break;
        case "japan":
          capitalSpan.textContent = "Tokyo";
          break;
        default:
          capitalSpan.textContent = "";
          break;
      }
    }
  </script>
</body>
</html>
```

**Question 8B: Convert text into a JavaScript object and display the result on a webpage**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Convert Text to JavaScript Object</title>
  <script>
    window.onload = function() {
      var text = '{"name" : "John", "age": 20, "city": "New York"}';
      var jsonObject = JSON.parse(text);
      document.getElementById("result").textContent = JSON.stringify(jsonObject, null, 2);
    };
  </script>
</head>
<body>
  <h2>Converted JavaScript Object</h2>
  <pre id="result"></pre>
</body>
</html>
```

<hr>

### 9A. Create a page that has one input, which can take multi-line text and a submit button. Once the user clicks the submit button, it should show the number of characters, words and lines in the text entered using an alert message. Words are seperated with white spaces and lines are sepearted with new line character. 

### 9B. The world is a dangerous place to live; not because of the people who are evil, but because of the people who dont do anything about it. - by Albert Einstine. Print this using blockquote in Bootstrap. 


**Question 9A: Create a page to analyze multi-line text input**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Text Analyzer</title>
  <script>
    function analyzeText() {
      var inputText = document.getElementById("textInput").value;
      var numCharacters = inputText.length;
      var numWords = inputText.split(/\s+/).filter(function(word) {
        return word !== '';
      }).length;
      var numLines = inputText.split(/\r\n|\r|\n/).filter(function(line) {
        return line !== '';
      }).length;
      alert("Number of characters: " + numCharacters + "\nNumber of words: " + numWords + "\nNumber of lines: " + numLines);
    }
  </script>
</head>
<body>
  <h2>Text Analyzer</h2>
  <textarea id="textInput" rows="5" cols="50"></textarea>
  <br>
  <button onclick="analyzeText()">Submit</button>
</body>
</html>
```

**Question 9B: Print a quote using blockquote in Bootstrap**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Blockquote Example</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<body>
  <h2>Quote by Albert Einstein</h2>
  <blockquote class="blockquote">
    <p class="mb-0">"The world is a dangerous place to live; not because of the people who are evil, but because of the people who don't do anything about it."</p>
    <footer class="blockquote-footer">Albert Einstein</footer>
  </blockquote>
</body>
</html>
```

<hr>

### 10A. Develop a script using jQuery to solve the following - 
### i. Limit charcter input in the text area including count. 
### ii. Based on check box, disable/enable the form submit button. 

### 10B. Demonstrate Making HTTP request in angular. 

**Question 10A: Develop a script using jQuery**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>jQuery Script</title>
  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
  <script>
    $(document).ready(function() {
      // Limit character input in textarea and show count
      $('#textInput').keyup(function() {
        var maxChars = 100; // maximum characters allowed
        var charCount = $(this).val().length;
        if (charCount > maxChars) {
          $(this).val($(this).val().substring(0, maxChars));
        }
        $('#charCount').text(charCount + '/' + maxChars);
      });

      // Disable/enable form submit button based on checkbox
      $('#agreeCheckbox').change(function() {
        $('#submitButton').prop('disabled', !$(this).prop('checked'));
      });
    });
  </script>
</head>
<body>
  <h2>jQuery Script</h2>
  <textarea id="textInput" rows="5" cols="50"></textarea><br>
  <span id="charCount">0/100</span><br><br>
  <input type="checkbox" id="agreeCheckbox"> Agree to terms<br><br>
  <button id="submitButton" disabled>Submit</button>
</body>
</html>
```


**Question 10B: Demonstrate Making HTTP request in Angular**

```typescript
// Import HttpClientModule in your Angular module

import { HttpClientModule } from '@angular/common/http';

@NgModule({
  declarations: [
    // Components, directives, pipes
  ],
  imports: [
    BrowserModule,
    HttpClientModule // Import HttpClientModule here
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

Now, you can make HTTP requests in your Angular components or services using HttpClient:

```typescript
import { HttpClient } from '@angular/common/http';

@Injectable({
  providedIn: 'root'
})
export class DataService {
  constructor(private http: HttpClient) { }

  fetchData() {
    return this.http.get('https://api.example.com/data');
  }
}
```

In this example, a service named DataService is created to make HTTP requests using HttpClient.
