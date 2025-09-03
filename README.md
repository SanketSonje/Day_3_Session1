# Emmet
Emmet is a toolkit for web developers that speeds up the process of writing HTML and CSS by using abbreviations that 
expand into full code snippets. It's a huge time-saver and helps you write code faster and more efficiently.

# 🔹 Why
- Saves time while writing repetitive HTML code.  
- Reduces typos by generating properly structured elements.  
- Makes writing nested structures quicker and more consistent.

Gist Link : https://gist.github.com/SanketSonje/21b5dacb8443c553591a22431aa36480

# Overview of Snippet Code
Writing the same HTML5 structure repeatedly is time-consuming.  
With a **VS Code snippet**, you can type a short prefix (e.g., `html5`) and instantly expand it into a complete boilerplate template.

## 🔹 Why
- Save time by avoiding repetitive typing.  
- Maintain consistency across projects.  
- Easily start new HTML files with best practices built-in.  

# Snippet Code

Add the following JSON inside your **VS Code user snippets** (`File > Preferences > User Snippets` → choose `html.json` or a global snippets file):

```json
{
  "HTML5 Boilerplate": {
    "prefix": "html5",
    "body": [
      "<!doctype html>",
      "<html lang=\"${1:en}\">",
      "<head>",
      "  <meta charset=\"utf-8\">",
      "  <meta name=\"viewport\" content=\"width=device-width, initial-scale=1\">",
      "  <title>${2:${TM_FILENAME_BASE}}</title>",
      "  <meta name=\"description\" content=\"${3:Page description}\">",
      "  <link rel=\"stylesheet\" href=\"${4:styles.css}\">",
      "</head>",
      "<body>",
      "  <header>",
      "    <h1>${5:Page Title}</h1>",
      "  </header>",
      "",
      "  <main>",
      "    $0",
      "  </main>",
      "",
      "  <script src=\"${6:script.js}\" defer></script>",
      "</body>",
      "</html>"
    ],
    "description": "HTML5 boilerplate (prefix: html5)"
  }
}

## How to Use
Open VS Code → Create a new HTML file.
Type html5 and press Tab / Enter.

## 🔹 Overview of JS debugging in VS Code
Debugging is the process of **finding and fixing errors** by running code step-by-step.  
VS Code has a built-in debugger that works seamlessly with Node.js for JavaScript projects.

---

## 🔹 Why
- Understand how the program executes.  
- Inspect variable values in real time.  
- Catch logic errors without relying only on `console.log()`.  

---

## 🔹 Code Example (`app.js`)

```js
// app.js
function add(a, b) {
  return a + b;
}

function multiply(x, y) {
  return x * y;
}

let num1 = 5;
let num2 = 10;

console.log("Starting program...");
let sum = add(num1, num2);
console.log("Sum:", sum);

let product = multiply(num1, num2);
console.log("Product:", product);
console.log("Program finished.");

#🔹 Steps to Debug in VS Code
Open this project in VS Code.
Create a folder named .vscode.
Inside .vscode, create a file named launch.json.
Add the configuration below.
The snippet expands into a full HTML5 boilerplate with placeholders

