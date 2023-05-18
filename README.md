# Resource:

## Managing your static site generator and content

---

**Initial workshop downloads**

Node.js - https://nodejs.org/en  
*(Node package manager should be included in node)*  
Visual Studio Code - https://code.visualstudio.com/  
GitBash (only Windows) - https://git-scm.com/download/win  
*  
PLUS: Make an account on gitlab - https://gitlab.com/  

---

**Starting node server, for development**

Start a terminal on your computer. On PC, start the program Git Bash, on Mac start the program Terminal. If you are not in the Cantina project folder, you can navigate there with ls ("list". Displays the files in the directory you are in), and cd ("change directory". Changes to the directory you type the name of—for example " cd Documents").  

Once the terminal is in the project's own directory, run the following command to start the node server.  

<code>npm run start</code>  

Then you can view the local site in the browser by going to http://localhost:8080/  

---

**Upload the site to the Internet**

Start another terminal in the project's directory and type

<code>npm run deploy</code>

This command takes all files in the _site folder and uploads them to the remote server. The site is then online.  

---

**Shut down server and terminal**

When you want to stop the server - possibly to restart it - you press *CTRL+C*  

And if you then want to close the terminal, type <code>exit</code>

---

**Other terminal commands:**

<code>clear</code> (Clears the screen in the terminal)  
<code>node -v</code> (Shows your node version (and that you have node installed correctly))  
<code>npm -v</code> (Shows your version of node package manager)  

---

## Eleventy Instructions

You must ALWAYS work in the <code>src</code> folder and NEVER in the <code>_site</code> folder. The <code>_site</code> folder contains the html that is generated from the <code>src</code> folder. ***You therefore always work from the <code>src</code> folder!***

***New page***  
If you want to create a new page, use one of the existing pages as a template, for example <code>index.md</code>
Note the top content on the page: <code>eleventyNavigation</code> describes the page as a menu link. <code>layout</code> describes which layout template the page uses.
***All layout templates are located under src/includes/layouts - and you can create new ones yourself as needed***  

***Collections***  
So far, the site has postCollection as the site's only content type. This content appears on the posts page. There is a template for a single post in the layouts folder. This template show how the content should be organised.

---


---

## Let's Suck at Static Site Generators Together
### Workshop break down  

_  

This is an introduction to Static Site Generators. The workshop presents a simple code base that gives the workshop participants an understanding of the core principles of Static Site Generators.  

This page is the workshop's knowledge and code base, and holds content that can help the participants in their work. the website's code can also be downloaded from here when the workshop begins.  
*  

**Intro. Presentation of technology and frameworks:** 
1. Static Site Generators 
2. Eleventy
3. Node.js
4. Markdown
5. Visual Studio Code
<br/><br/>

---

**1)**

**Static Site Generators**

First - What is a **static site generator**?... Websites can generally be divided into two categories - static and dynamic. A static site is much like it sounds - static, fixed, constant. This means that the site is designed, stored on a server and delivered to the user's web browser as is. It doesn't toggle between the point where the developer hits the "Save" button and when the end user clicks it. Developers create the content using HTML, format it with CSS, and upload the static page to a server where it remains unchanged and ready for access via a browser request.  

Conversely, dynamic websites are in an almost constant state of change and are typically powered by a CMS. The CMS literally builds each page as needed each time a user clicks on it. Developers create content that is stored in a back-end database. When a user requests a URL, the CMS-powered website retrieves the relevant content from the database, loads an HTML template, renders the content in the template, and returns a formatted HTML page to the visitor's browser—a process known as server-side processing.  

Read: https://www.netlify.com/blog/2020/04/14/what-is-a-static-site-generator-and-3-ways-to-find-the-best-one/  

Video intro: https://www.youtube.com/watch?v=3INXQ_4W42g
<br/><br/>  

---

**2)**

**Eleventy (11ty)**

Eleventy (or 11ty) is a Node.js based static site generator (SSG). SSGs render a set of static HTML, CSS, and JavaScript files that are then uploaded to the web. The site is therefore less dependent on server technologies.  

This provides several important advantages:  
_ Hosting is simple: you display almost exclusively HTML.  
_ The system is secure: there is nothing to hack.  
_ Performance is optimal as everything is rendered in advance.  

11ty website: https://www.11ty.dev/  
<br/><br/>

---

**3)**

**Node.js**

Node.js is a server-side platform built on Google Chrome's JavaScript Engine (V8 Engine). Node.js was developed by Ryan Dahl in 2009.  

Node.js is an open source platform and runtime environment for developing servers and network applications. Node.js applications are written in JavaScript and can be run within the Node.js runtime on OS X, Microsoft Windows, and Linux.  

Node.js also offers a rich library of various JavaScript modules, which greatly simplifies the development of web applications using Node.js.  

Intro to node.js (video, Dan Shiffman): https://www.youtube.com/watch?v=RF5_MPSNAtU
<br/><br/> 

---

**4)**

**Markdown**

Markdown is a lightweight *markup language* that you can use to add formatting to plain text documents. Markdown was created by John Gruber in 2004 and is now one of the world's most popular markup languages.  

Using Markdown is different than using a WYSIWYG editor. In a program like Microsoft Word, you click buttons to format words and sentences, and the changes are visible immediately. Markdown is different: When you create a Markdown-formatted file, you add Markdown syntax to the text to specify which words and phrases should look different.  

Link to intro: https://www.markdownguide.org/  

video intro: https://www.youtube.com/watch?v=f49LJV1i-_w&t=197s
<br/><br/>

---

**5)**

**Visual Studio Code**

Visual Studio Code is a freeware code editor made by Microsoft for Windows, Linux and macOS. Features include support for debugging, syntax highlighting, intelligent code completion, snippets, code conversion, and integrated Git. Users can change the theme, keyboard shortcuts, preferences and install extensions that add additional functionality.  

Intro video: https://www.youtube.com/watch?v=S320N3sxinE
<br/><br/>

---

**Ressourcer:**

Let's Learn Eleventy!  
https://www.learnwithjason.dev/lets-learn-eleventy  

Google webfont helper tool (for embedding webfonts without having to pull them from Google's servers = self hosted): https://google-webfonts-helper.herokuapp.com/fonts  