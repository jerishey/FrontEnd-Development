# HTML
HTML (HyperText Markup Language) is the standard language for creating and structuring web pages using tags and elements. It defines how content like text, images, and links appear in a browser.

## Features :
```bash
1. Simple & Easy → HTML uses basic tags and syntax, making it very easy for beginners to learn and start building web pages quickly.

2. Platform Independent → HTML works on all operating systems and browsers, so your webpage can run anywhere without modification.

3. Multimedia Support → It allows embedding images, audio, and videos directly into web pages, making content more interactive and engaging.

4. Hyperlinking → HTML provides linking through anchor tags, enabling users to navigate between pages and websites easily.

5. Structured Content → It organizes content using headings, paragraphs, lists, and tables, ensuring proper layout and readability.

6. Forms Support → HTML enables creation of forms to collect user data like login details, feedback, and registrations.
```
## Example :
```bash
<!DOCTYPE html>
<html>
<head>
    <title>My First Webpage</title>
</head>
<body>
    <h1>Welcome to My Webpage</h1>
    <p>This is my first paragraph of text!</p>
</body>
</html>
```
### Understanding the Structure of an HTML Page :
```bash
1. HTML is used to create the structure of a webpage.

2. Every HTML file starts with <!DOCTYPE html> to tell the browser it’s an HTML5 document.

3. The <html> tag contains all other elements of the page.

4. The <head> section stores information like the page title and metadata.

5. The <body> section contains all the visible content such as text, images, and links.

6. After writing the code, save the file with a .html extension so browsers can recognize it.

7. Open the file in any browser like Chrome or Firefox to see it displayed.

8. The browser reads and interprets the HTML code, converting it into a visual webpage.

9. Each HTML tag is processed so elements like headings, paragraphs, and images appear correctly.

10 The final webpage shows all the content on the screen, and any HTML errors may affect how it looks.
```

## 1. HTML Editors
An HTML Editor is a software application designed to help users create and modify HTML code. It often includes features like syntax highlighting, tag completion, and error detection, which facilitate the coding process.
```bash
There are two main types of HTML editors:

1. Text-Based Editors - Allow direct coding with features like syntax highlighting and code completion for full control over the webpage structure. Example - Sublime Text, Visual Studio Code, etc.

2. WYSIWYG (What You See Is What You Get) Editors - Offer a graphical interface to design web pages visually, automatically generating the corresponding HTML code. Example - Adobe Dreamweaver, etc.
```
### HTML Editors List :
There are various free and paid HTML editors available in the market, but in this article, we will be covering some renowned free HTML editors that you can use as a beginner or switch to if you are an experienced developer.
```bash
1. Notepad : Notepad is a simple text editor that is also used to write HTML code. It is an inbuilt desktop application available in Windows OS.

2. Sublime Text Editor : Sublime is a cross-platform code editor tool. It supports all markup languages and is used as an editor for HTML. Similar to the Notepad editor, create a new file and save it with a .html extension to run an HTML file.

3. Visual Studio Code : It is one of the most popular code editors of today's generation. Many companies and software developers prefer this online HTML code editor.
```
### Reasons to Use an HTML Editor :
Editors for HTML offer several advantages to writing and editing HTML codes. Some benefits of using HTML editors are:
```bash
1. Syntax Highlighting: HTML editors use color-coding to distinguish tags, attributes, and content, making code more readable.

2. Autocompletion: These editors suggest tags and correct common errors, improving coding speed.

3. Code Validation: Built-in validators check for syntax issues and missing tags.

4. Debugging Tools: Some editors offer debugging features to identify and fix errors.

5.Customization Options: Customize the interface and settings to enhance your coding experience.
```

### How to Choose the Right HTML Editor? :
```bash
1. Skill level: Beginners might prefer WYSIWYG editors for ease of use, whereas advanced users may opt for text-based editors for better control.

2. Project needs: Larger projects might benefit from a more robust editor with extensive features and integrations.

3. Compatibility: Ensure the editor supports other technologies you plan to use like CSS, JavaScript, or various frameworks.
```

## 2. HTML Comments :
HTML comments are used to add notes or explanations in the HTML code that are not displayed by the browser.

- They are useful for documenting the code, making it easier to understand and maintain.
- To add a comment, use the syntax <!-- your comment here -->.
```bash
<!-- This is a comment and will not be displayed on the webpage -->
<p>This is visible text.</p>
```
### Different Ways to Add Comments in HTML :
```bash
1. Single-Line and Inline Comments : Single-line and inline comments are used to add short notes or explanations within code without affecting its execution.

2. Multi-Line Comments and Hidden Code Sections : Multi-line comments and hidden code sections let developers write detailed explanations or temporarily disable code without deleting it.
```
<b>Example :</b>
<i>

Single-Line and Inline Comments
```bash
<html>
<body>
    <!--This is heading Tag-->
    <h1>Single Line Comment</h1>
    <!--This is single line comment-->
    <h2>This is <!--given for--> single line comment</h2>
</body>
</html>
``` 
Multi-Line Comments and Hidden Code Sections
```bash
<html>
<body>
    <!-- This is
         heading tag -->
    <h1>Multiple Line Comment</h1>
    <!-- This is
    multi-line
         comment -->
    <h2>This is multi-line comment</h2>
    <!-- <button style="font-family: Sans-serif;">
           Click Me
         </button> -->

</body>
</html>
```
</i>

### Uses of HTML Comments :
```bash
1. Code Organization: Comments can help break up sections of code, making it easier to navigate, especially in larger projects.

2. Collaboration: When working with others, comments are crucial for explaining why certain HTML elements are used, or for leaving instructions for team members.

3. Debugging: Temporarily disabling parts of HTML code by commenting them out is a common use, allowing developers to isolate issues.

4. Documentation: Providing details or documentation within the code for future reference without the need for external documentation.
```
<br>

## 3. HTML Elements
HTML elements are the basic building blocks of a webpage, defining its structure and content using start tags, content, and end tags.
```bash
1. Every HTML element begins with an opening tag and ends with a closing tag.

2. Elements can contain text, attributes, or other nested elements.

3. Some elements are self-closing (e.g., <br>, <img>).

4. The browser reads elements to render the page visually.

5. Proper nesting of elements ensures valid and accessible HTML.
```
<b>Example :</b>
```bash
<!-- HTML code to illustrate HTML elements -->

<!DOCTYPE html>
<html>

<head>
    <title>HTML Elements</title>
</head>

<body>
    <p>Welcome to webpage!</p>
</body>

</html>
```
<b>About HTML Elements :</b>
```bash
- Syntax

1. An opening tag indicates where the content begins: <tagname>.
2. A closing tag indicates where the content ends: </tagname>.
3. The actual content resides between the opening and closing tags.

- Case Sensitivity

1. HTML tags are not case-sensitive. For example, <B> and <b> both represent bold text.
2. However, it’s a best practice to use lowercase tags for consistency and readability.
```
### Block-Level Elements and Inline Elements :
In HTML, elements are broadly categorized into two main types based on how they display in the document layout: block-level elements and inline elements.

<i>
<br>

Block-Level Elements
```bash
1. Block-Level Elements : Block-level elements start on a new line, occupy the full available width, stack vertically, and can contain both block-level and inline elements.

Examples

- <div>: A general-purpose container for other elements.
- <p>: Defines a paragraph.
- <h1>, <h2>, ..., <h6>: Heading elements of different levels.
- <ol>, <ul>: Ordered and unordered lists.
- <table>: Defines a table.
- <form>: Used for HTML forms to collect user inputs.
- <section>, <article>, <nav>, <aside>, <header>, <footer>: Semantic elements that define areas of a webpage.
```
Inline Elements
```bash
2. Inline Elements : Inline elements do not start on a new line, take only the width of their content, and are used within block-level elements to add or style content.

Examples

- <span>: A general-purpose inline container for phrasing content.
- <a>: Creates hyperlinks.
- <img>: Embeds an image.
- <strong>, <b>: Used for strong emphasis and bold text, respectively.
- <em>, <i>: Used for emphasis and italic text, respectively.
- <br>: Inserts a line break within text.
- <input>: Creates interactive controls for forms.
```
</i>
<br>

## 4. HTML Attributes
HTML Attributes are special words used within the opening tag of an HTML element. They provide additional information about HTML elements. HTML attributes are used to configure and adjust the element's behaviour, appearance, or functionality in a variety of ways.

<b>Features :</b>
```bash
- Provide Additional Information → Attributes give extra details about HTML elements (e.g., href, src).

- Always in Opening Tag → Attributes are written inside the start tag of an element.

- Work in Name–Value Pairs → Written as name="value" (e.g., class="box").

- Customize Elements → Control behavior, style, or functionality of elements.

- Support Global Usage → Some attributes like id, class, style can be used with most elements.

- Enable Linking & Media → Attributes like href (links) and src (images/videos) connect resources.

- Case Insensitive (HTML5) → Attribute names are not case-sensitive in HTML5.

- Multiple Attributes Allowed → One element can have more than one attribute at the same time.
```
<b> Example: </b>
```bash
<a href="https://example.com" target="_blank">Visit Website</a>

<img src="image.jpg" alt="Sample Image" width="200">

<p style="color: blue;">This is a paragraph</p>

<input type="text" placeholder="Enter your name">
```
<b> Explaination: </b>
```bash
1. href → Specifies the link destination
2. target="_blank" → Opens link in a new tab
3. src → Defines image source
4. alt → Alternative text for image
5. style → Adds inline styling
6. type & placeholder → Define input behavior
```
### Types of HTML Attributes :
```bash
1. Global Attributes : These attributes can be used with any HTML element (though their effects might vary based on the element).

2. Event Attributes - These define the actions to be taken on specific browser events.

3. Input Attributes - Specific to input elements within <form> tags.

4. Image Attributes - Specific to the <img> element for handling images.

5. Link Attributes - Specific to linking elements like <a> and <link>.

6. Table Attributes - Used with table elements like <table> , <th> , <tr> , and <td>.

7. Style Attributes - Define styles directly on an element.

8. Media Attributes - Related to media elements like <audio> and <video>.

9. Accessibility Attributes - Help improve accessibility, such as alt for images and aria-* attributes.

10. Meta Attributes - Used with meta elements to specify metadata like  charset.
```
<b> Explaination : </b>
<i>

Global Attributes
```bash
1. id → (Global) Uniquely identifies an element
2. class → (Global) Groups elements for styling or scripting
3. style → (Global) Applies inline CSS styles
4. title → (Global) Displays tooltip text on hover
5. hidden → (Global) Hides an element from display
6. tabindex → (Global) Controls tab navigation order
```
Event Attributes
```bash
1. onclick → (Event) Executes script when element is clicked
2. onmouseover → (Event) Executes when mouse is over element
3. onmouseout → (Event) Executes when mouse leaves element
4. onchange → (Event) Executes when value changes
5. onload → (Event) Executes when page or element loads
```
Input Attributes
```bash
1. type → (Input) Defines type of input field
2. value → (Input) Sets default input value
3. placeholder → (Input) Shows hint text in input
4. required → (Input) Makes field mandatory
5. readonly → (Input) Makes field non-editable
6. disabled → (Input) Disables input field
7. checked → (Input) Pre-selects checkbox/radio
8. name → (Input) Identifies form data
```
Image Attributes
```bash
1. src → (Image) Specifies image source
2. alt → (Image) Provides alternative text
3. width → (Image) Sets image width
4. height → (Image) Sets image height
```
Link Attributes
```bash
1. href → (Link) Specifies URL of link
2. target → (Link) Defines where to open link
3. download → (Link) Forces file download
4. rel → (Link) Defines relationship of linked resource
```
Table Attributes
```bash
1. colspan → (Table) Merges multiple columns
2. rowspan → (Table) Merges multiple rows
3. border → (Table) Defines table border
```
Style Attributes
```bash
style → (Style) Applies inline CSS styling
```
Media Attributes
```
1. controls → (Media) Displays media controls
2. autoplay → (Media) Starts media automatically
3. loop → (Media) Repeats media playback
4. muted → (Media) Mutes media sound
```
Accessibility Attributes
```bash
1. alt → (Accessibility) Describes image for screen readers
2. aria-label → (Accessibility) Provides accessible label
3. aria-hidden → (Accessibility) Hides element from screen readers
```
Meta Attributes
```bash
1. charset → (Meta) Defines character encoding
2. name → (Meta) Specifies metadata name
3. content → (Meta) Provides metadata value
```
</i>

### Important Points About HTML Attributes :
```bash
1. Use Lowercase
- Always write attributes in lowercase for better readability and consistency
- It follows modern HTML5 standards and improves code clarity

2. Use Quotes for Values
- Always use quotes (" ") around attribute values to avoid errors
- Especially important when values contain spaces or special characters

3. Use Consistent Quotes
- Use either single (' ') or double (" ") quotes, but be consistent
- Double quotes are commonly used in most HTML code examples

4. Boolean Attributes
- Boolean attributes do not need values (e.g., disabled, checked)
- If present, they are automatically considered true

5. Maintain Attribute Order
- Keep a consistent order like id, class, then other attributes
- Helps in writing clean, readable, and maintainable code

6. Avoid Deprecated Attributes
- Avoid old attributes like align, bgcolor, border
- Use CSS instead for styling and better modern practices
```

## 5. HTML DOCTYPE Declaration
HTML DOCTYPE (Document Type Declaration) is an instruction that appears at the beginning of an HTML document, before the <html> tag.
<br>

<b> Features :</b>
```bash
1. Its primary role is to tell the web browser which version of HTML the page is written in, ensuring that the browser renders the content correctly.

2. It is not an HTML tag, but rather a special instruction that specifies how the browser should interpret the HTML.

3. It is recommended to always use <!DOCTYPE html> at the top of your HTML file for HTML5.
```
<b> Example : </b>
```bash
<!DOCTYPE html>
<html>
<body>
    <p>welcome to my website</p>
</body>
</html>
```
### What Happens Without DOCTYPE html
```bash
1. Quirks Mode Activation: Browsers may switch to quirks mode, leading to outdated behaviors that cause inconsistent rendering compared to standards mode.

2. Rendering Issues: CSS properties like box-sizing, margins, and widths may be interpreted differently, causing layout problems and misaligned elements that are difficult to debug.

3. Cross-Browser Inconsistencies: Different browsers might render the page differently in quirks mode, making it hard to achieve cross-browser consistency.

4. CSS and JavaScript Problems: Modern features like Flexbox, Grid, and certain JavaScript methods may not work correctly, causing compatibility issues.

5. Unpredictable Behavior: Without <!DOCTYPE>, rendering becomes unpredictable, making debugging more challenging and leading to unpredictable page behavior when adding new features.
```

## 6. HTML Headings
HTML headings are used to define the titles and subtitles of sections on a webpage. They help organize the content and create a structure that is easy to navigate.

- Proper use of headings enhances readability by organizing content into clear sections.
- Search engines utilize headings to understand page structure, aiding in SEO.

### Levels of HTML Heading Tags
HTML offers six levels of heading tags, each serving a different purpose in structuring your content:
```bash
1. <h1> – Main Heading (Largest)
- Represents the primary focus of the page, usually used for the main title.
- Use only one <h1> tag per page for the best SEO practices.
- Makes it clear to both users and search engines what the main topic is.

2. <h2> – Subheadings
- Ideal for dividing the content into major sections.
- If the content has further subsections, use <h3> to create a logical flow.

3. <h3> to <h6> – Smaller Headings
- These heading levels are used for finer subdivisions, gradually decreasing in size and importance.
- <h3> is used for subsections under <h2>, while <h4> to <h6> are used for additional, less important subdivisions.
- <h6> defines the least important heading.
```
<b> Example : </b>
```bash
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" 
          content="width=device-width, initial-scale=1.0">
    <title>HTML</title>
</head>
<body>
    <h1>This is the Main Heading</h1>
	<h2>This is a Subheading</h2>
	<h3>This is a Smaller Subheading</h3>
	<h4>This is a Sub-Subheading</h4>
	<h5>This is a Minor Subheading</h5>
	<h6>This is the Smallest Heading</h6>
</body>
</html>
```
### Best Practices for Using HTML Headings :
```bash
1. Use Only One <h1> per Page: The <h1> tag should be reserved for the main title of the page. Too many <h1> tags can confuse both users and search engines about the content’s priority.

2. Maintain a Logical Structure: Follow a logical hierarchy of headings (<h1> → <h2> → <h3>) to ensure content is organized. Don't jump directly from <h1> to <h4>, as it can make the content harder to navigate.

3. Keep Headings Descriptive: Headings should clearly describe the content that follows. This makes it easier for readers to understand what each section is about.

4. Avoid Overusing Heading Tags: Headings are for organizing content, not for styling text. Use them where appropriate and avoid using heading tags for emphasis or styling alone.
```

## 7. HTML Paragraphs
A paragraph in HTML is simply a block of text enclosed within the `<p>` tag. The `<p>` tag helps divide content into manageable, readable sections. It’s the go-to element for wrapping text in a web page that is meant to be displayed as a distinct paragraph.

- Adds space before and after the paragraph to visually separate it from other content.
- Breaks the text into a single block, creating an easy-to-read section.

### Properties of the paragraph Tag :
```bash
1. The browser reduces multiple spaces added by users to a single space.

2. If a user adds various lines, the browser compresses them into one line.

3. By default, the display of the paragraph element is set to "block," meaning each new paragraph is placed on a new line.
```
<b> Example : </b>
```bash
<!--<!DOCTYPE html>-->
<!--<html lang="en">-->

<!--<head>-->
<!--    <title>The p tag</title>-->
<!--</head>-->

<!--<body>-->
<!--need to comprase this-->
    <p>A Computer Science portal for geeks.</p>
    <p>It contains well written, well thought articles.</p>
<!--</body>-->

<!--</html>-->
```
## 8. HTML Links Hyperlinks
HTML Links, also known as Hyperlinks, are used to connect one web page to another, allowing users to navigate easily between different pages, websites, or sections within the same page.

- The `<a>` (anchor) tag creates hyperlinks, using the href attribute to specify the destination URL.
- It can link text, images, or buttons for navigation.
- Links can open in the same tab or a new tab using the target attribute, and other common attributes include title for additional information.

<b> Syntax : </b>
```bash
<a href="URL">Link Text</a>
```

### Important Attributes :
```bash
1. href (Hyperlink Reference) : The href attribute specifies the destination URL of the link. It tells the browser where to go when the user clicks the link. Without href, the anchor tag will not function as a proper link.

Example :
<a href="https://example.com">Go to Example</a>

2. target : The target attribute defines where the linked document will open. It helps control whether the link opens in the same tab or a new tab/window.

Example:
<a href="https://example.com" target="_blank">Open in New Tab</a>

3. title : The title attribute provides additional information about the link. This text is displayed as a tooltip when the user hovers over the link.

Example:
<a href="https://example.com" title="Go to Example Website">Example</a>
```

### Types of Links 
```bash
1. External Link : An external link connects to a different website outside your current domain. It is commonly used to reference other websites or resources.

Example:
<a href="https://google.com">Google</a>

2. Internal Link : An internal link connects to another page within the same website. It helps in navigating between different pages of a site.

Example:
<a href="about.html">About Page</a>

3. Email Link : An email link allows users to open their email client and send a message directly to a specified email address.

Example:
<a href="mailto:example@gmail.com">Send Email</a>

4. Anchor Link (Same Page) : An anchor link is used to jump to a specific section within the same webpage. It improves navigation, especially on long pages.

Example:
<a href="#section1">Go to Section 1</a>
```
### Example: 
```bash
<!DOCTYPE html>
<html>
<head>
    <title>HTML Links Example</title>
</head>
<body>

    <h2>HTML Links Demo</h2>

    <!-- External Link -->
    <p>
        <a href="https://www.google.com" target="_blank" title="Go to Google">
            Visit Google
        </a>
    </p>

    <!-- Internal Link -->
    <p>
        <a href="about.html" title="Go to About Page">
            Go to About Page
        </a>
    </p>

    <!-- Email Link -->
    <p>
        <a href="mailto:example@gmail.com" title="Send an Email">
            Send Email
        </a>
    </p>

    <!-- Anchor Link (Same Page) -->
    <p>
        <a href="#section1">
            Go to Section 1
        </a>
    </p>

    <br><br>

    <!-- Target Section -->
    <h3 id="section1">Section 1</h3>
    <p>This is Section 1 of the same page.</p>

</body>
</html>
```

## 9. HTML Images
The HTML `<img>` tag is used to embed an image in web pages by linking them. It creates a placeholder for the image, defined by attributes like src, width, height, and alt, and does not require a closing tag.

There are two ways to insert the images into a webpage:
- By providing a full path or address (URL) to access an internet file.
- By providing the file path relative to the location of the current web page file.

<b> Syntax :</b>
```bash
<img src="image.jpg" alt="Description of image">
```
### Important Attributes
```bash
1. src (Source) : The src attribute specifies the path or URL of the image. It tells the browser where to find the image file.

2. alt (Alternative Text) : The alt attribute provides a description of the image. It is displayed if the image fails to load and is important for accessibility (screen readers).

3. width and height : The width and height attributes in the <img> tag define the size of an image, with values specified in pixels by default.

- Control the displayed width and height of an image.
- Values are specified in pixels.
- Help maintain consistent layout and prevent page shifting.

4. title : The title attribute adds a tooltip to an image that appears when a user hovers over it.

- Displays descriptive text on mouse hover.
- Added using the title attribute in the <img> tag.
```
<b> Example :</b>
```bash
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML</title>
</head>
<body>
    <img src="Image.png" alt="GFG image" />
</body>
</html>
```

## 10. HTML5 Semantics
HTML5 semantic elements provide meaningful tags that clearly describe their purpose, improving readability, accessibility, and SEO for both humans and browsers.

- Clearly define the role and content of elements.
- Improve code readability and structure.
- Enhance accessibility for screen readers.
- Help browsers and search engines understand page content.
- Examples include `<form>`, `<table>`, `<article>`, `<header>`, and `<footer>`.

### Semantic Elements
```bash
1. The <article> Tag : The <article> tag represents independent, self-contained content that can be reused or distributed separately, such as blog posts, news articles, or forum entries. It should make sense even when viewed outside the main webpage.

2. The <aside> Tag : The <aside> tag is used for content that is indirectly related to the main content, such as sidebars, advertisements, or related links. It is usually displayed alongside the main content.

3. The Details and Summary Tag : The <details> tag is used to create a collapsible section that can be shown or hidden by the user. The <summary> tag defines a visible heading or title for the <details> content that users can click to expand or collapse.

4. The Figure and Figcaption Tag : The <figure> tag is used to group media content like images, diagrams, or illustrations. The <figcaption> tag provides a caption or description for the content inside <figure>, improving clarity and accessibility.

5. The Header Tag : The <header> tag defines the introductory section of a webpage or a section. It typically contains headings, logos, navigation links, or other introductory content.

6. The Footer Tag : The <footer> tag represents the bottom section of a webpage or a section. It usually contains information such as copyright details, contact information, or related links. Multiple <footer> elements can exist on a single page. 

7. The Main Tag : The <main> tag defines the main content of the webpage. It should contain unique content that is directly related to the central topic of the page and should not include repeated elements like headers or footers.

8. The Section Tag : The <section> tag is used to divide content into thematic groups or sections, such as introduction, services, or contact information. Each section typically includes a heading.

9. The nav Tag : The <nav> tag is used to define a set of navigation links, such as menus, tables of contents, or navigation bars that help users move through the website.

10. The Mark Tag : The <mark> tag is used to highlight or emphasize specific text within a paragraph, making it stand out visually for the user.
```

### Best Practices for Using HTML5 Semantic Elements
```bash
1. Do not overuse <div> : Use semantic elements where appropriate instead of non-semantic <div> elements to provide more specific information about the content.

2. Structure content logically : Organize the content within semantic elements to reflect the meaning and importance of the information.

3. Validate your HTML : Use tools like the W3C HTML Validator to ensure that your use of semantic elements adheres to HTML5 standards.
```
<b> Example : </b>
```bash
<!DOCTYPE html>
<html>
<head>
    <title>Semantic HTML Example</title>
</head>
<body>

    <!-- Header Section -->
    <header>
        <h1>My Website</h1>
        <p>Welcome to my semantic webpage</p>
    </header>

    <!-- Navigation Menu -->
    <nav>
        <a href="#">Home</a> |
        <a href="#">About</a> |
        <a href="#">Contact</a>
    </nav>

    <!-- Main Content -->
    <main>

        <!-- Section -->
        <section>
            <h2>Blog Section</h2>

            <!-- Article -->
            <article>
                <h3>My First Blog</h3>
                <p>This is my first blog post using semantic HTML.</p>
            </article>

            <article>
                <h3>My Second Blog</h3>
                <p>This is another article example.</p>
            </article>
        </section>

        <!-- Aside (Sidebar) -->
        <aside>
            <h3>Related Links</h3>
            <p>Check out more articles here.</p>
        </aside>

        <!-- Figure with Caption -->
        <figure>
            <img src="https://via.placeholder.com/200" alt="Sample Image">
            <figcaption>This is a sample image</figcaption>
        </figure>

        <!-- Details & Summary -->
        <details>
            <summary>Click to see more info</summary>
            <p>This content can be hidden or shown.</p>
        </details>

        <!-- Highlight Text -->
        <p>This is an example of <mark>highlighted text</mark>.</p>

    </main>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 My Website | Contact: example@gmail.com</p>
    </footer>

</body>
</html>
```

## 11. HTML Entities
HTML Entities are special codes used to display reserved characters, symbols, or invisible spaces in a webpage that cannot be typed directly or have special meanings in HTML (like <, >, or &).

<b> Features : </b>
```bash
1. Used to display special characters that HTML normally reserves.
2. Always start with & and end with ; (example: &lt; for <).
3. Help avoid errors or misinterpretation in HTML code.
4. Commonly used for symbols, non-breaking spaces, and mathematical signs.
5. Make web content more readable and properly formatted.
```
<b> Example : </b>
```bash
<!DOCTYPE html>
<html>
<head>
  <title>HTML Entities Example</title>
</head>
<body>
  <h2>Using HTML Entities</h2>
  
  <p>Less than symbol: &lt;</p>
  <p>Greater than symbol: &gt;</p>
  <p>Ampersand symbol: &amp;</p>
  <p>Copyright symbol: &copy; 2025 MyWebsite</p>
  <p>Registered symbol: &reg; Trademark</p>
  <p>Non-breaking space example: Hello&nbsp;World</p>

</body>
</html>
```
### Commonly Used HTML Entities
HTML entities are used to display special characters and reserved symbols that cannot be written directly in HTML.
<br>
<i>

`1. Reserved Characters`

| Character | Entity Name | Description  |
| --------- | ----------- | ------------ |
| `<`       | `&lt;`      | Less than    |
| `>`       | `&gt;`      | Greater than |
| `&`       | `&amp;`     | Ampersand    |
| `"`       | `&quot;`    | Double quote |
| `'`       | `&apos;`    | Single quote |

`2. Space & Formatting`

| Character | Entity    | Description        |
| --------- | --------- | ------------------ |
| (space)   | `&nbsp;`  | Non-breaking space |
| –         | `&ndash;` | En dash            |
| —         | `&mdash;` | Em dash            |

`3. Currency Symbols`

| Symbol | Entity     | Description  |
| ------ | ---------- | ------------ |
| ₹      | `&#8377;`  | Indian Rupee |
| $      | `&dollar;` | Dollar       |
| €      | `&euro;`   | Euro         |
| £      | `&pound;`  | Pound        |

`4. Common Symbols`
| Symbol | Entity     | Description          |
| ------ | ---------- | -------------------- |
| ©      | `&copy;`   | Copyright            |
| ®      | `&reg;`    | Registered trademark |
| ™      | `&trade;`  | Trademark            |
| °      | `&deg;`    | Degree               |
| ×      | `&times;`  | Multiplication       |
| ÷      | `&divide;` | Division             |

</i>

### Best Practices for Using HTML Entities
```bash
1. Use Named Entities When Possible: Named entities (&lt; instead of &#60;) are easier to remember and make your code more readable.

2. Verify Entity Codes: Always check your entity codes to ensure they display correctly across all browsers and platforms.

3. Use Entities for Readability and Compliance: Besides reserved characters, use entities to improve the readability of your code and to comply with HTML standards, especially when dealing with characters that may not be directly supported by your page’s charset.
```

## 12. HTML Symbols
HTML symbols are special characters used to display characters not on the keyboard or that might conflict with HTML code.

- Use named entities like `&lt; for < and &gt; for >`.
- Use number entities like `&#60; for < and &#62; for >`.

### Commonly Used HTML Symbols
```bash
1. ©:copyright sign: The © symbol, called the copyright sign, indicates that the creator owns the rights to a work, protecting it from unauthorized use or reproduction.

- Syntax : &copy;

2. ®:registered trade mark sign: The ® symbol, called the registered trademark sign, shows that a brand, logo, or name is officially registered with the government and legally protected from unauthorized use.

- Syntax : &reg;

3. ™:trade mark sign: The ™ symbol, called the trademark sign, indicates that a word, logo, or symbol is being claimed as a trademark, even if it is not officially registered.

- Syntax : &trade;

4. @: at symbol sign: The @ symbol, called the "at" sign, is commonly used in email addresses to separate the username from the domain and also in social media to mention or tag someone.

- Syntax : &commat;

5. ¶: paragraph sign : The ¶ symbol, called the paragraph sign or pilcrow, is used to mark the beginning of a new paragraph or to reference specific paragraphs in a text.

- Syntax : &para;

6. §:section sign: The § symbol, called the section sign, is used to reference a particular section of a document, law, or book for easy citation.

- Syntax : &sect;

7. ℂ: double-struck capital c: The ℂ symbol, called double-struck capital C, is mainly used in mathematics to represent the set of all complex numbers.

- Syntax : &copf;

8. ℅: care of: The ℅ symbol, called "care of," is used in addresses to indicate that correspondence should be delivered via another person or entity.

- Syntax : &incare; 

9. ℊ:script small g : The ℊ symbol, called script small g, is mainly used in mathematics and physics to represent specific variables or functions, often in a stylized or formal notation.

- Syntax : &gscr;

10. ℋ: script capital h : The ℋ symbol is used in mathematics and physics for special functions or notations.

- Syntax : &hamilt; 

11. ℕ: &nopf; : The ℕ symbol represents the set of natural numbers in mathematics.

- Syntax : &nopf;

12. №: numero sign : The № symbol is used to indicate “number” in lists or documents.

- Syntax : &numero;

13. ★ : black star : The ★ symbol is used for ratings, highlights, or decoration in text.

- Syntax : &starf;

14. ☎: black telephone : The ☎ symbol represents a phone or contact information.

- Syntax : &phone;

15. ☆: white star : The ☆ symbol is used for outlines, highlights, or decorative points.

- Syntax : &star;

16. ♀ : female sign : The ♀ symbol denotes female gender in biology or social contexts.

- Syntax : &female;

17.  ♂:male sign : The ♂ symbol denotes male gender in biology or social contexts.

- Syntax : &male;

18. ♪: eighth note : The ♪ symbol represents a musical note in notation.

- Syntax : &sung;

19. ✓:check mark : The ✓ symbol, called the check mark, is used to indicate correctness, completion, approval, or confirmation.

- Syntax : &check

20. ✗:ballot x : The ✗ symbol, called the ballot X, is used to indicate a wrong answer, rejection, cancellation, or disapproval in forms, lists, or documents.

- Syntax : &&cross;
```