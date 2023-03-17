# JavaScript best practices

## General practices

1. Keep all the JavaScript code in JS files, not in the `script` tag.
2. Keep your [code clean](https://devinduct.com/blogpost/22/javascript-clean-code-best-practices) following this advice about:
  - type checks.
  - naming.
  - simplicity.
  - DRY.
3. If you use node modules, .lock files should be in the repository to avoid problems with future versions of the dependencies.
4.  If you use ES6, use object destructuring to get the values from an object. This way you can avoid repeating a lot of code.

## JavaScript in the browser


1. Do not commit `console.log` to your repo. It’s ugly, it kills performance and it can make confidential data be visible to anyone using the browser tools to look at your website.
2. Do not use `window.alert()` or `window.confirm()`. It’s ugly, impossible to style, it stops code execution and displays differently on different browsers. Use custom modal instead.
3. Keep the number of changes/updates to the DOM as low as possible, they are very expensive for the browser.
4. Keep the application logic separated from DOM manipulation tasks.
5. Do not use `document.write` or `eval`
6. Add `node_modules` dir to your .gitignore file as all those files are not needed in your repo (each team member will install all packages thanks to your package.json file).
7. Do not commit old pieces of code as inline comments. They will make your project look messy. If you need to review a previous version of your code, you can always use git history.

------