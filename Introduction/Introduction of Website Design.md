# Introduction
## Welcome & Curriculum Overview
HTML (Hyper Text Markup Language) and CSS (Cascading Style Sheets) are the core building blocks of web design. Here’s a beginner-friendly look at each of these technologies and how they work together to make websites functional and visually appealing.
### Basic HTML Tags
Here's a breakdown of some basic HTML tags you’ll likely use on every webpage:

html

- `<html>`: The root element that wraps the entire HTML document.

- `<head>`: Contains metadata, like the title, links to stylesheets, and other non-visual information.

- `<title>`: Sets the title of the page displayed on the browser tab.

- `<body>`: Contains all visible content on the page.

- `<h1>, <h2>,... <h6>`: Headings, where `<h1>` is the most important and `<h6>` the least.

- `<p>`: Paragraphs, used for blocks of text.

- `<a href="URL">`: Anchor tags, used to create links. href is the attribute that specifies the link’s URL.

- `<img src="image.jpg" alt="description">`: Image tag, with src specifying the image file and alt providing a description for accessibility.

- `<ul>` and `<ol>`: Unordered and ordered lists. Inside these tags, 

    - `<li>` elements represent each item in the list.

# Basic HTML Example
``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Webpage</title>
</head>
<body>
    <h1>Welcome to My Webpage!</h1>
    <p>This is my first paragraph in HTML.</p>
    <a href="https://example.com">Click here to visit Example.com</a>
    <img src="image.jpg" alt="A sample image">
</body>
</html>
```
# What is CSS?
CSS is used to style the HTML content, allowing you to change the colors, fonts, spacing, and layout of your webpage. With CSS, you can make your site more visually appealing and align with specific design choices.

## Basic CSS Syntax

CSS consists of selectors and declarations:

   - Selector: Specifies which HTML element(s) the styles should apply to (e.g., h1, p, body).
   - Declaration: Includes properties and values, such as color: red; or font-size: 16px;. Declarations are placed within curly braces {} and separated by semicolons.
### Ways to Add CSS to HTML
``` html
<p style="color: blue;">This text is blue.</p>
```
### Internal CSS: 
- Written in the `<style>` tag within the `<head>`- section of your HTML file.
``` html
    <style>
        body {
            background-color: #f0f0f0;
        }
        h1 {
            color: green;
        }
    </style>
``` 
### External CSS: 
In a separate .css file, linked in the HTML `<head>` section.
``` html
html
<link rel="stylesheet" href="styles.css">
```
``` css 
css
body {
    background-color: #f0f0f0;
}
h1 {
    color: green;
}
```
### Basic CSS Example

``` css
body {
    background-color: #e0f7fa; /* Light blue background */
}

h1 {
    color: #00796b; /* Dark teal text */
    font-family: Arial, sans-serif; /* Font for heading */
}

p {
    font-size: 16px;
    color: #333;
``` 
### HTML & CSS Together
When you combine HTML and CSS, your webpage gains structure and style. Here’s a simple example:

### * HTML (index.html)
``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Styled Webpage</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Welcome to My Styled Webpage!</h1>
    <p>This is a paragraph with custom styling applied.</p>
</body>
</html>
```
### * CSS (styles.css)
``` css
body {
    background-color: #fafafa;
    font-family: Arial, sans-serif;
}

h1 {
    color: #2196f3;
    text-align: center;
}

p {
    color: #666;
    font-size: 18px;
    line-height: 1.6;
}
```
## Key Points to Remember
- HTML is for structure: It organizes the content with tags.
- CSS is for styling: It makes the content look good by changing colors, fonts, layout, etc.
- External CSS is preferred: Keeping CSS in a separate file is a best practice because it makes it easier to manage and apply consistent styles across multiple pages.
- Experimentation is key: Try adding new tags and styles to your projects, checking how each element and style change affects the page.

## Getting Started
To start experimenting with HTML and CSS:

    1. Open a simple code editor (like VS Code, Atom, or even Notepad).
    2. Save your HTML file as index.html and your CSS file as styles.css.
    3. Open index.html in a browser to see your changes in action!

As you get more comfortable, try building a simple project like a personal webpage or a portfolio. It’s a fantastic way to apply what you learn and start seeing your skills grow.

# •	How The Web Works
The web works as a global network of computers that communicate with each other to provide access to websites, information, and online services. 

Here’s a brief breakdown of how it functions:

## Clients and Servers

- Client: This is usually your device (computer, smartphone, or tablet) with a browser (like Chrome, Firefox, or Safari) that requests and displays web content.
- Server: A powerful computer that stores and serves websites to clients. Each website is hosted on a server, which responds to client requests for specific content.
## Web Addresses and DNS

- Websites have unique URLs (Uniform Resource Locators), like https://example.com, which users enter to access specific sites.
- URLs are translated into IP addresses (unique identifiers for devices on the internet) by the Domain Name System (DNS). DNS is like an internet “phonebook” that matches domain names with IP addresses, so users don’t need to remember complex IP numbers.
## HTTP and HTTPS

- HTTP (Hypertext Transfer Protocol) is the language or protocol used for communication between clients and servers. When you enter a URL, your browser sends an HTTP request to the server to fetch the webpage.
- HTTPS is a secure version of HTTP, encrypting data for safer transmission, especially important on sites where sensitive information (like passwords) is involved.
## Request and Response

- When you visit a website, your browser sends an HTTP request to the web server for specific content.
- The server processes this request and sends back an HTTP response that includes the requested HTML, CSS, JavaScript, and any other files (like images).
- The browser then interprets these files and displays the webpage.
## Rendering Web Pages

- After receiving a response, the browser processes the HTML structure, applies CSS for styling, and executes JavaScript for interactivity.
- The rendering engine in the browser turns all this data into a visually organized and interactive webpage.
## Databases

- For more complex sites, such as social media or e-commerce, servers interact with databases to store and retrieve data (e.g., user accounts, products).
- When you perform an action (like logging in), the server accesses the database, retrieves the information, and displays it as part of the webpage.
## CDNs (Content Delivery Networks)

- Many websites use CDNs to store copies of data (like images, videos, and scripts) on servers around the world. 
- This improves website speed and performance by delivering content from the nearest server to the user.

In short, the web is a complex network where clients request content, servers respond with data, and browsers interpret that data to display websites. This process is enabled by protocols (like HTTP), DNS for finding IPs, and tools like CDNs and databases for efficient data management and delivery.

# •	The Roles of HTML, CSS, and JS
In website design, HTML, CSS, and JavaScript (JS) each play distinct roles that work together to create visually appealing, interactive, and functional websites. Here’s how each contributes to a web page:

1. HTML (HyperText Markup Language)

    - Role: Structure and Content
    - Function: HTML is the foundation of a webpage. It provides the basic structure and organizes content by marking it up with tags.
    - Elements: Headings, paragraphs, lists, images, links, forms, tables, and other types of content are added to a page using HTML tags.

Example:
``` html
<h1>Welcome to My Website</h1>
<p>This is a paragraph of text about the website.</p>
<img src="logo.png" alt="Site logo">
```

- Analogy: Think of HTML as the “skeleton” of a webpage, defining the essential parts that make up the content.
2. CSS (Cascading Style Sheets)
- Role: Styling and Presentation
- Function: CSS is used to style and visually enhance the HTML content. It controls colors, fonts, layout, spacing, and positioning of elements on the page.
- How It Works: CSS is typically written in a separate file and linked to the HTML. It applies rules to HTML elements using selectors to make the page look attractive and aligned with a brand or theme.
- Example:
``` css
body {
    background-color: #f0f0f0;
    font-family: Arial, sans-serif;
}
h1 {
    color: #333;
    text-align: center;
}
p {
    font-size: 16px;
    color: #666;
}
```
- Analogy: CSS is like the “skin and clothes” of a webpage, defining its appearance and style.
3. JavaScript (JS)
- Role: Interactivity and Functionality
- Function: JavaScript adds dynamic behaviors to a webpage, making it interactive and responsive to user actions. It can handle form validations, animations, interactive elements, and retrieve data from servers (using AJAX or APIs) without refreshing the page.
- How It Works: JavaScript is usually linked to HTML files and can manipulate HTML and CSS in response to events, like button clicks or scrolling.
- Example:
``` js
document.querySelector("button").addEventListener("click", function() {
    alert("Button clicked!");
});
``` 
- Analogy: JavaScript is like the “muscle and brain” of a webpage, adding functionality and responsiveness to user actions.
# Summary of Roles:

- HTML = Structure and Content
- CSS = Styling and Visual Presentation
- JavaScript = Interactivity and Dynamic Functionality

Together, HTML, CSS, and JavaScript provide a complete set of tools to build structured, stylish, and interactive websites, creating an engaging user experience.
# •	Installing The Tools We Need for website design
To start with website design and development, you’ll need a few essential tools. Here’s a simple guide to installing them:
1. Text Editor or Code Editor

- A code editor is where you’ll write your HTML, CSS, and JavaScript. There are many free and popular options that provide syntax highlighting, extensions, and debugging tools.
- Recommended Editors:
    - [Visual Studio Code](https://code.visualstudio.com/Download) (VS Code): A free, powerful, and customizable code editor by Microsoft. It’s great for beginners and professionals alike.
    - Sublime Text: A fast and lightweight editor with a clean interface, although some features require a paid license.
- How to Install:
    - Visit the editor’s website (e.g., [Visual Studio Code](https://code.visualstudio.com/Download)).
    - Download the installer for your operating system (Windows, macOS, or Linux).
    - Run the installer and follow the instructions to complete the setup.

2. Web Browser

    - Browsers display your website and allow you to test and debug your code. Modern browsers come with developer tools, which help you inspect elements, view console logs, and debug code.
    - Recommended Browsers:
        - Google Chrome: Popular and powerful, with excellent developer tools.
        - Mozilla Firefox: Known for strong privacy features and robust developer tools.
        - Microsoft Edge: Based on Chromium, similar to Chrome, and also has solid developer tools.
    - How to Install:
        - For Chrome, go to [Google Chrome](https://www.google.com/intl/en_uk/chrome/dr/download/?brand=YTUH&gad_source=1&gclid=Cj0KCQiA88a5BhDPARIsAFj595jV2ekQnXrklgVtpbcZZfUVf3wU_UTzTPTyQyLpyqTRCntdb1Xycm8aAqKyEALw_wcB&gclsrc=aw.ds), download, and install.
        - For Firefox, go to [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/new/), download, and install.
        - For Edge, it’s pre-installed on Windows, or you can download it from Microsoft Edge.

3. Version Control (Optional, but Highly Recommended)

    - Git: Git is a version control system that lets you track changes, collaborate with others, and manage different versions of your project.

    - GitHub: An online platform to store Git repositories and collaborate with others.

    - How to Install Git:
        - Visit [Git’s website](https://git-scm.com/downloads) and download the installer.
        - Run the installer, following the prompts to complete the setup.
        - Once installed, you can access Git through your command line (Terminal on macOS/Linux, Command Prompt or Git Bash on Windows).

4. Package Managers (Optional)

    - Node.js and npm: Node.js allows you to run JavaScript on your computer (outside the browser) and comes with npm (Node Package Manager) to install libraries and tools.
    - How to Install Node.js and npm:
        - Go to [Node.js](https://nodejs.org/en/download/prebuilt-installer).
        - Download the recommended version for your operating system.
        - Run the installer and follow the prompts. This will install both Node.js and npm.

5. Preprocessors and Frameworks (Optional)

    - As you advance, you may want to work with tools like Sass (a CSS preprocessor) or frameworks like Bootstrap/tailwind for faster design.
    - Most of these can be installed via npm after you’ve installed [Node.js](https://nodejs.org/en/download/prebuilt-installer).

6. Design Tools (Optional)

    - Figma or Adobe XD: These are popular design tools for creating and prototyping website layouts and designs.
    - How to Access:
        - Sign up on [Figma](https://www.figma.com/) or [Adobe XD](https://helpx.adobe.com/ca/xd/) websites. Both offer free plans for beginners.

Quick Summary:

- Text Editor: Install VS Code.
- Browser: Use Chrome, Firefox, or Edge.
- Version Control (Git): Optional, but useful for tracking changes.
- Node.js and npm: Optional, for installing libraries.
- Design Tools: Optional, try Figma or Adobe XD for design work.

Once you have these tools, you’re ready to start coding, testing, and designing websites!
# Configuring VS Code for web development
Configuring Visual Studio Code (VS Code) for web development can improve productivity and make coding more efficient and enjoyable. Here’s a step-by-step guide to set up VS Code for HTML, CSS, and JavaScript development:
1. Install VS Code

- Download and install VS Code from the official website.
- Follow the installation prompts specific to your operating system (Windows, macOS, or Linux).

2. Basic Configuration

- Open Settings: Go to File > Preferences > Settings (or press Ctrl + , on Windows/Linux or Cmd + , on macOS) to access settings.
- Set Up Auto-Save: In Settings, search for “Auto Save” and enable it (set it to afterDelay or onWindowChange) to automatically save changes.
- Format on Save: In Settings, search for “Format On Save” and enable it to automatically format your code each time you save.

3. Install Useful Extensions

- Extensions add functionality to VS Code. Here are some helpful extensions for web development:

    - HTML, CSS, and JavaScript Essentials:
        - HTML Snippets: Provides HTML code snippets for faster coding.
        - Prettier: A popular code formatter for clean and consistent formatting.
        - Live Server: Launches a local server that auto-reloads your browser when you save changes, allowing you to see updates instantly.
        - CSS Peek: Allows you to jump directly to CSS definitions in your stylesheets.
        - JavaScript (ES6) Code Snippets: Adds JavaScript snippets for faster coding, especially useful for ES6 syntax.

    - Additional Useful Extensions:
        - Path Intellisense: Autocompletes file paths, making it easier to link images, scripts, or styles.
        - Color Highlight: Highlights colors in your CSS files.
        - Bracket Pair Colorizer 2: Colors matching brackets, making it easier to read nested code.
        - GitLens: Adds advanced Git features within VS Code for easy version control.

    - How to Install Extensions:
        - Click on the Extensions icon on the sidebar (or press Ctrl + Shift + X on Windows/Linux or Cmd + Shift + X on macOS).
        - Search for each extension by name and click Install.

4. Set Up Live Server

    - After installing Live Server, right-click on your index.html file and select Open with Live Server. This will open your HTML file in the browser and reload the page whenever you save changes.
    - You can also launch it by clicking Go Live at the bottom of the VS Code window.

5. Enable Emmet for HTML and CSS

    - Emmet is a tool built into VS Code that lets you write HTML and CSS faster with shortcuts and abbreviations.
    - For example, typing div.container and pressing Tab will expand it to 
    ``` html 
        <div class="container"></div>
    ```
    - You don’t need to install anything—Emmet is enabled by default in VS Code for HTML and CSS files.

6. Set Up Code Formatting

    - Prettier: After installing Prettier, configure it as your default formatter.
        - Go to File > Preferences > Settings.
        - Search for “default formatter” and set it to Prettier.
        - Enable Format On Save by searching for it in the settings and checking the box.
    - This will format your code each time you save, keeping HTML, CSS, and JavaScript code organized.

7. Configure Settings for Specific File Types

    - VS Code allows you to apply settings based on the file type. Here’s how to set preferences for HTML, CSS, and JavaScript files:
        - Open your Settings (JSON) by selecting Settings and then clicking on the icon in the upper right corner ({}).
        - Add configuration options like this:
``` json
        {
            "[html]": {
                "editor.defaultFormatter": "esbenp.prettier-vscode"
            },
            "[css]": {
                "editor.defaultFormatter": "esbenp.prettier-vscode"
            },
            "[javascript]": {
                "editor.defaultFormatter": "esbenp.prettier-vscode"
            }
        }
```
8. Set Up Git Integration (Optional)

    - If you’re using Git for version control, VS Code has built-in Git support. Click on the Source Control icon in the sidebar.
    - To initialize a repository, click Initialize Repository and follow the prompts. You can manage commits, branches, and other Git functions directly from VS Code.

9. Customize the Interface (Optional)

    - Go to File > Preferences > Color Theme to choose a theme that suits your style.
    - Explore File > Preferences > Icon Theme to change the icon set in the sidebar for better visuals and organization.

## Summary of Key Extensions & Configurations:

    - Install Extensions: Live Server, Prettier, HTML/CSS/JavaScript snippets, and others for productivity.
    - Enable Auto-Save and Format on Save.
    - Set Prettier as the default formatter for consistent formatting.
    - Launch Live Server to see real-time changes.

With this setup, you’re ready to start web development in VS Code with a productive, streamlined workflow!



