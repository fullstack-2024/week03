## Build a Cool Website: A Step-by-Step Guide to HTML & CSS

Ready to unleash your inner web developer? This lab will guide you through building a simple website using HTML and CSS. You'll learn how to structure the website using HTML tags and then style it with CSS to create a visually appealing and responsive design. Let's dive in!

**What you'll need:**

* **A text editor:** Sublime Text, Atom, or Visual Studio Code are popular choices.
* **A web browser:** Chrome, Firefox, or Safari are all great options.
* **A little creativity and a willingness to learn!**

**Our Mission:**

By the end of this lab, you'll be able to:

* Understand the basic structure of HTML documents.
* Use CSS to style different elements on your website.
* Create a responsive layout that adapts to different screen sizes.

**Let's get started!**

**Step 1: Building the Foundation (HTML)**

1. **Create a New File:** Open your text editor and create a new file named `index.html`. This will be the main file for your website.
2. **Set the Stage:** Add the following code to your `index.html` file:

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Your Awesome Website</title>
       <link rel="stylesheet" href="styles.css">
   </head>
   <body>
       </body>
   </html>
   ```

   - Replace "Your Awesome Website" with your desired title.
   - Don't forget to create a `styles.css` file later!

3. **Structure Your Site:** Now, let's add the different sections of your website:

   ```html
   <header>
       <h1>Welcome to Your Website!</h1>
   </header>
   <nav>
       <ul>
           <li><a href="#home">Home</a></li>
           <li><a href="#about">About</a></li>
           <li><a href="#services">Services</a></li>
           <li><a href="#contact">Contact</a></li>
       </ul>
   </nav>
   <main>
       <article>
           <h2>Your Story</h2>
           <p>Share something awesome about yourself or your website!</p>
       </article>
       <aside>
           <h2>Cool Stuff</h2>
           <p>Show off your latest projects, hobbies, or anything else you're passionate about.</p>
       </aside>
   </main>
   <footer>
       <p>&copy; 2024 Your Name. All rights reserved.</p>
   </footer>
   ```

   - Replace the content with your own text and images.
   - Use appropriate HTML tags like `<h1>` for main headings, `<h2>` for subheadings, and `<p>` for paragraphs.

**Step 2: Styling Your Masterpiece (CSS)**

1. **Create the CSS File:** In the same directory as your `index.html`, create a new file named `styles.css`. This is where the magic happens!
2. **Start with the Basics:** Add the following code to your `styles.css` file:

   ```css
   body {
       margin: 0; /* Remove default margin */
       font-family: Arial, sans-serif; /* Set a nice font */
   }
   ```

3. **Style It Up!** Now comes the fun part:

   - **Header & Footer:** Make them stand out with a background color and centered text:

     ```css
     header, footer {
         background-color: #333;
         color: white;
         text-align: center;
         padding: 20px;
     }
     ```

   - **Navigation:** Make it sleek and easy to use:

     ```css
     nav {
         background-color: #666;
         padding: 10px 0; /* Top and bottom padding */
     }

     nav ul {
         list-style: none; /* Remove default list styling */
         padding: 0;
         display: flex; /* Use flexbox for horizontal layout */
         justify-content: center; /* Center items horizontally */
     }
     nav ul li {
  margin: 0 10px; /* Spacing between list items */
    }
    nav ul li a {
  color: white;
  text-decoration: none;
  padding: 5px 10px;
  border-radius: 5px; /* Rounded corners */
  transition: background-color 0.3s ease; /* Smooth hover effect */
}

nav ul li a:hover {
  background-color: #999;
}
```

