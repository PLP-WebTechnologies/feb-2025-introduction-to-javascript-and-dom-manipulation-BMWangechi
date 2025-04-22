# Introduction to JavaScript and DOM Manipulation

## Objectives

Write basic JavaScript functions.
Manipulate the DOM dynamically.
Respond to user interactions.

## Instructions

- Create a script.js file and link it to a HTML.
- Structure the document using DOCTYPE, html, head, and body.

>[!NOTE]
>  - Write JavaScript that:
>  - Changes text content dynamically.
>  - Modifies CSS styles via JavaScript.
>  - Adds or removes an element when a button is clicked.


# Tasks
- Create a well-structured HTML5 document.
- Use at least 5 different HTML elements.
- Ensure semantic correctness.

Happy Coding! 💻✨

Answers

<!DOCTYPE html>
<html lang="en"
<head>
    <meta charset="UTF-8"
    meta name="viewport" content="width=device width, initial scale=1.0"
    <title>DOM Manipulation</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1 id="main title"> Wangechi's Website</h1>
    </header>
    <main>
        <p id="description">This is a simple example of DOM manipulation using JavaScript.</p>
        <button id="change-text-btn">Change Text</button>
        <button id="toggle-element-btn">Toggle Element</button>
        <div id="dynamic-element" style="display: none;">I am a dynamically toggled element!</div>
    </main>
    <footer>
        ; 2025 My Website</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>        

// Change text content dynamically
document.getElementById('change-text-btn').addEventListener('click', function() {
    document.getElementById('main-title').textContent = 'Text Changed!';
    document.getElementById('description').textContent = 'The text content has been updated dynamically.';
});

// Modify CSS styles via JavaScript
document.getElementById('change-text-btn').addEventListener('click', function() {
    document.getElementById('main-title').style.color = 'blue';
    document.getElementById('description').style.fontStyle = 'italic';
});

// Add or remove an element when a button is clicked
document.getElementById('toggle-element-btn').addEventListener('click', function() {
    const dynamicElement = document.getElementById('dynamic-element');
    if (dynamicElement.style.display === 'none') {
        dynamicElement.style.display = 'block';
    } else {
        dynamicElement.style.display = 'none';
    }
});

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    text-align: center;
}

header, footer {
    background-color: #f8f8f8;
    padding: 20px;
}

main {
    padding: 20px;
}

button {
    margin: 10px;
    padding: 10px 20px;
    font-size: 16px;
}
