# Tailwind Demo Guide
 
# Tailwind Setup

https://tailwindcss.com/

### Tailwind 3.0

**Legacy Version** New Version is available (4.0) 

**Guide for Tailwind 3.0**: https://www.youtube.com/watch?v=lCxcTsOHrjo&ab_channel=DaveGray

### Tailwind 4.0

1. Install [node.js](https://nodejs.org/en), [vscode](https://code.visualstudio.com/)
2. Install Tailwind CSS
    
    Install `tailwindcss` and `@tailwindcss/cli` via npm.
    
    ```bash
    npm install tailwindcss @tailwincss/cli
    ```
    
3. Create a `build` and `src` directory/folder
    1. Put `input.css` or whatever name you like into `src` folder
    2. Put the main html file `index.html` into your `build` folder
4. Import Tailwind in your CSS
    
    Add the `@import "tailwindcss";` import to your main CSS file (`input.css` from the previous step.
    
    ```bash
    @import "tailwindcss";
    ```
    
5. Start the Tailwind CLI build process
    
    Run the CLI tool to scan your source files automatically for classes and build your CSS. 
    
    **Note**: change `input.css` to whatever you used as your main css file and `output.css` can be any name you like.
    
    ```bash
    npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
    ```
    
6. Start using Tailwind in your HTML
    
    Add your compiled CSS file to the `<head>` and start using Tailwind’s utility classes to style your content
    
    ```html
    <!doctype html>
    <html>
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <link href="./output.css" rel="stylesheet">
    </head>
    <body>
      <h1 class="text-3xl font-bold underline">
        Hello world!
      </h1>
    </body>
    </html>
    ```
    
7. **Final Check**

This is what your project directory should look like this repository after following these steps. `README.md`, `LICENSE`, `.gitattributes` can be ignored.

[output.css](src/output.css), [input.css](src/input.css), [index.html](build/index.html)

---

## Additional Setups

- Install [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VSCode
    - Go to settings of the extension, search `full reload` check the setting (this is so that the page refreshes so css changes can take effect)
- Install [Tailwind CSS IntelliSence](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss) in VSCode

---

# Tailwind Documentation

You can visit the docs to browse the documentation, but it’s often helpful to use the search function and just search whatever style that you need. 

- **Shortcut**: `ctrl + k`
- Link to docs → https://tailwindcss.com/docs/styling-with-utility-classes
    

---

# Tailwind Tip and Tricks
