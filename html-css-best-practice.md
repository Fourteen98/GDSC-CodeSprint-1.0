# HTML & CSS best practices

1. Use the appropriate tags for each element (e.g., links, titles, etc.) and use HTML5 semantic tags (e.g., header, nav) over `div`s.
2. Avoid lines of code that are too long (100 characters or more).
3. Be careful with blank lines and indentation.
    - Do not add blank lines, spaces, or indentations without a reason.
    - For readability, add blank lines to separate large or logical code blocks.
    - For readability, add two spaces of indentation. Do not use the tab key.
      - on some code editors, you can set the tab button to do an `X` amount of spaces.
4. Close all HTML elements.
     - `<div>` always needs `</div>`
5. Use lowercase for elements and attribute names.
     - use `<div>` not `<DIV>`
     - use `<div class="striped">` not  `<div CLASS="striped">`
7. Always quote attribute values.
     - use `<div class="striped">` not  `<div class=striped>`
8. Use space-less equal signs.
     - use `<div class="striped">` not  `<div class = "striped">`
9. Do not use inline styles. Keep your style definition in a separate CSS file.
10. Do not overuse `!important` rule in your CSS style definitions.
11. Always use the class attribute for multiple elements (do not use ID selector for multiple elements).
12. If you want to create a CSS rule for multiple elements, use a class attribute instead. For example, instead of using `color: #3498db;` 3 times
    ```CSS
        #intro1 {color: #3498db; font-size: 10px; font-weight: bold;}
        header {color: #3498db; font-size: 20px; background-color: green;}
        #banner {color: #3498db; font-size: 30px; background-image: url(images/static.jpg);}
    ```
    you can create a class and add it to all element that need to be blue.
    
    ```CSS
       .blue {color: #3498db;}
    ```
14. Do not commit old pieces of code as inline comments. They will make your project look messy. If you need to review a previous version of your code, you can always use git history.

------
