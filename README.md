# Module-4-Coding-Assignment
git clone https://github.com/yourusername/html-css-js-assignment.git
2. Folder Structure:
Create the folder structure for the assignment:

plaintext
Copy code
html-css-js-assignment/
├── index.html
├── style.css
└── script.js
3. HTML File (index.html):
Create the basic HTML structure. Here’s an example:

html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript Practice</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Welcome to the JavaScript Practice Assignment</h1>
    <script src="script.js"></script>
</body>
</html>
4. CSS File (style.css):
You can style your page (this step is optional, but it makes your page nicer). For example:

css
Copy code
body {
    font-family: Arial, sans-serif;
    text-align: center;
}

h1 {
    color: #333;
}
5. JavaScript File (script.js):
The core of this project will be the JavaScript code. You need to create an array of names and loop through it, checking the first letter of each name. Based on that letter, print the appropriate message in the console.

Steps:

Create an array of names.
Loop through the array.
Check if the first letter of the name is "J" or "j".
Print "Goodbye [Name]" if true, otherwise print "Hello [Name]".
Here’s an example of how the script.js might look:

javascript
Copy code
// List of names
var names = ["John", "Jane", "Mark", "Sara", "Tom", "James", "Lucas"];

// Loop through the names
for (var i = 0; i < names.length; i++) {
    var firstLetter = names[i].charAt(0).toLowerCase(); // Get the first letter of the name
    
    // Check if the name starts with 'j' or 'J'
    if (firstLetter === "j") {
        console.log("Goodbye " + names[i]);
    } else {
        console.log("Hello " + names[i]);
    }
}
Explanation:

charAt(0).toLowerCase() is used to get the first letter of each name and convert it to lowercase, so we can handle both "J" and "j" uniformly.
The for loop iterates through the names array and checks the condition for each name.
6. Test the Project:
Open index.html in a browser.
Open the Developer Tools in your browser (F12 or right-click -> "Inspect").
Go to the "Console" tab to see the output.
The output should print either "Hello [Name]" or "Goodbye [Name]" for each name in the array.
7. Push the Changes to GitHub:
After testing your solution locally, you can push the changes to your GitHub repository:

bash
Copy code
git add .
git commit -m "Complete JavaScript Practice Assignment"
git push origin main
