# CSS 
CSS stands for Cascading Style Sheets. It is a stylesheet language used to style and enhance website presentation. CSS is one of the three main components of a webpage, along with HTML and JavaScript.
<br>

- HTML adds Structure to a web page.
- CSS adds the style and makes it visually appealing.
- JavaScript adds interactivity and logic to the page.

## Features : 
```CSS
1. Separation of content and design – keeps HTML structure separate from styling, making code cleaner and easier to maintain.

2. Reusability – one CSS file can style multiple pages, saving time and ensuring consistency across a website.

3. Selectors – allow precise targeting of elements (by tag, class, id, etc.) for flexible and efficient styling.

4. Responsive design – enables websites to automatically adjust layout and design for mobile, tablet, and desktop screens.

5. Rich styling options – supports colors, fonts, spacing, shadows, gradients, and modern visual effects.

6. Flexbox & Grid layouts – provide powerful tools to create responsive and well-structured page layouts easily.
```
## 1. Adding CSS to HTML - 3 Approaches
Each method serves a different purpose based on how you organize and manage your styles.

- Helps you structure CSS according to your project needs.
- Makes your code easier to maintain and update.
- Allows flexibility in applying styles to different parts of a webpage.
- Improves readability and reusability of your design.

### 1. Inline CSS
Inline CSS applies styles directly to HTML elements using the style attribute, allowing for quick, unique styling without external stylesheets.

#### Features :
```CSS
1. Quick Application: Ideal for rapid, one-off style adjustments.

2. High Specificity: Overrides other CSS rules due to its specificity.

3. Limited Reusability: Not suitable for applying the same styles to multiple elements.

4. Inline Styling: The style attribute within the <p> tag applies CSS directly to the paragraph, setting the text color to blue and font size to 18 pixels.

5. Immediate Effect: This method allows for quick, element-specific styling without the need for external or internal CSS.
```
#### When to Use Inline CSS ?
```CSS
1. Applying Unique Styles: Ideal for styling individual elements without affecting global styles.

2. Testing or Debugging: Useful for quick style adjustments during development.

3. Email Templates: Ensures consistent styling across various email clients.

4. Dynamic Styling with JavaScript: Allows for programmatically changing styles based on user interactions.
```
#### Example :
```CSS
# Centering Text with Inline CSS

<html>
<body>
    <div style="text-align: center; font-family: Arial, sans-serif;">
        <h2>Welcome to My Website</h2>
        <p>Enjoy your stay!</p>
    </div>
</body>
</html>
```
#### Advantages :
```CSS
1. Using style attributes we can provide styles directly to our HTML elements.

2. Inline CSS Overrides external and internal styles with higher specificity.

3. No need to create and upload a separate document as in the external style.

4. Inline styles have high specificity, allowing precise control over individual elements.

5. Enables dynamic style changes using JavaScript or server-side logic.

6. Inline styles don't require separate CSS files, potentially reducing HTTP requests.
```
#### Disadvantages :
```CSS
1. Adding style attributes to every HTML element is time-consuming.

2. Styling multiple elements can increase your page's size and download time, impacting overall page performance.

3. Reduced separation of concerns between HTML structure and CSS.

4. Inline styles cannot be used to style pseudo-elements and pseudo-classes.

5. It can be difficult to maintain consistency and make global style updates.
```

### 2. Internal CSS
Internal CSS is a method for defining CSS styles directly within an HTML document. It's particularly useful for applying unique styles to a single web page, and it's embedded within the `<style>` element located in the `<head>` section of the HTML file.

#### How to Use Internal CSS ?
Internal CSS is used to style a single HTML page by writing CSS inside the `<style>` tag within the `<head>` section.
```CSS
<!DOCTYPE html>
<html>

<head>
    <title>Internal CSS</title>
    <style>
        /* Internal CSS  */
        h1 {
            color: green;
            font-size: 50px;
            text-align: center;
        }

        p {
            color: blue;
            font-size: 25px;
            line-height: 1.5;
            text-align: center;
        }
    </style>
</head>

<body>
    <h1>Internal CSS</h1>
    <p>A Computer Science Portal..!</p>
</body>

</html>
```

#### Advantages of Internal CSS :
```CSS
1. Localized Styling: Keeps styles within the HTML file, avoiding conflicts with other pages and making it easier to manage styles at the local level.

2. Higher Specificity: Internal CSS has higher specificity than external CSS, allowing easier overriding of external styles within the same HTML file.

3. Performance: Reduces HTTP requests, potentially enhancing performance as no additional CSS files need to be loaded.

4. Ease of Implementation: Simple to use and implement, making it easy to quickly apply styles to a single page
```

#### Disadvantages of Internal CSS :
```CSS
1. Repetition: Styles must be repeated in multiple HTML files if the same styles are needed across different pages.

2. Increased File Size: Embedding CSS in HTML increases the file size of the HTML document.

3. Reduced Reusability: Limited code reusability across different web pages.

4. Limited Management: Managing styles across multiple pages can become difficult without a centralized stylesheet.
```

### 3. External CSS
External CSS is a method of styling web pages where all the CSS code is written in a separate .css file and linked to one or more HTML files using the <link> tag. It allows developers to control the design, layout, colors, fonts, and responsiveness of multiple web pages from a single file, making websites more organized, consistent, and easier to maintain.

#### How to Link an External CSS to HTML :
To link an external CSS file to an HTML document, you need to use the <link> element within the <head> section of your HTML file. The <link> element should have the rel attribute set to "stylesheet" and the href attribute specifying the path to your CSS file.

```CSS
<link rel="stylesheet" href="path/to/your/styles.css">
```
<b> Examplaination : </b>
```CSS
1. rel (Relationship) : Specifies the relationship between the current HTML document and the linked file.

2. href (Hyperlink Reference) : Defines the path or URL of the external CSS file.

3. type (MIME Type) : Specifies the type of the linked document.

4. media (Media Query Support) : Defines which device or screen the CSS is intended for.
```

#### Example :
```CSS
# HTML
<!DOCTYPE html>
<html>

<head>
    <title>External CSS</title>
    <link rel="stylesheet" href="styles.css">
</head>

<body>
    <h2>Welcome to Webpage</h2>
</body>

</html>

# CSS
/* Create a file named styles.css */

h2 {
    color: green;
    font-size: 20px;
}
```
#### Advantages of External CSS :
```CSS
1. Improved Maintainability: Having styles in a separate file makes it easier to manage and update your styles without modifying each HTML document.

2. Enhanced Reusability: The same CSS file can be linked to multiple HTML files, promoting consistent design across your site.

3. Efficient Caching: Browsers cache external CSS files, leading to faster page load times on subsequent visits.
```
#### Disadvantages of External CSS :
```CSS
1. Loading Time: Pages may not render correctly until the external CSS file is fully loaded, potentially causing a flash of unstyled content (FOUC).

2. Performance Concerns: Linking multiple CSS files can increase download times, affecting overall site performance.

3. Versioning and Caching Challenges: Large-scale projects may encounter difficulties in versioning and caching, leading to inconsistencies in styles.
```

## 2. CSS Syntax
CSS syntax defines how CSS rules are written so that browsers can interpret and apply them to HTML elements. It is useful for styling and designing web pages efficiently.

- It defines how styles are applied to HTML elements.
- It uses selectors to target elements.
- It consists of properties and values inside a declaration block.

### Explanation :

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20251018150341183638/diagram_of_a_css_rule.webp">

```CSS
1. Selector: Targets the HTML element "h1" to apply styles.

2. Declaration Block: Enclosed in curly braces { }, contains one or more declarations.

3. Property: Specifies the style attribute, here "color" for text color.

4. Value: Defines the property's setting, here "blue" for the text hue.

5. Overall Structure: Forms a complete CSS rule: h1 { color: blue; }, styling h1 headings blue.
```

### Example :
```CSS
<html>
<head>
    <style>
        /* CSS Rule */
        h1 {
            color: blue;
            /* Property: value */
            font-size: 24px;
        }

        p {
            color: green;
            font-size: 16px;
        }
    </style>
</head>

<body>
    <h1>Hello, World!</h1>
    <p>This is a simple paragraph.</p>
</body>
</html>
```

## 3. CSS Comments
CSS comments are used to add notes or explanations to your code, helping you and others understand it better.

### Features :
```CSS
1. Comments can be added anywhere in the code, and they can span across multiple lines.

2. It’s a good practice to add comments to clarify complex parts of your code for future reference or collaboration.

3. Older methods like <!-- --> for hiding CSS in older browsers are outdated and not recommended.

4. Comments are simply ignored by the browser, so they don't affect the output in any way.
```

### Types of Comments :
<i>
Single-line Comment

```CSS
<!DOCTYPE html>
<html>

<head>
    <title>Single line comment</title>
    <style>
        h1 {
            color: green;
        }

        /* Single line comment */
    </style>
</head>

<body>
    <h1>Study portal</h1>
    <p> Study portal for CS students</p>
</body>

</html>
```

Multiline Comment
```CSS
<!DOCTYPE html>
<html>

<head>
    <title>Multiline Comment</title>
    <style>
        h1 {
            color: green;
        }

        /* This is a multiline
           comment */
    </style>
</head>

<body>
    <h1>Study portal</h1>

    <p> A Computer Science portal </p>
</body>

</html>
```
</i>

## 4. CSS Ruleset
A CSS ruleset is the foundation of how styles are applied to HTML elements on a web page. It consists of a selector and one or more declarations, which define how elements are displayed.

### Explanation :
```CSS
1. A CSS ruleset is made up of a selector and declarations.

2. The selector targets HTML elements to apply styles.

3. Declarations are pairs of property names and values that define how the selected elements should be styled.

4. The declarations are enclosed in curly braces {}.

- Example:

<html><head>
    <style>
        /* This is a CSS ruleset */
        p {
            color: blue;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <p>This is a paragraph.</p>
</body></html>

5. The selector is p, which targets all <p> (paragraph) elements in the HTML.

6. The declarations define how the <p> element should look. The color property changes the text color to blue, and the font-size property sets the text size to 16px.
```

## 5. CSS Selectors
CSS Selectors are patterns used in CSS to select and target HTML elements so that styles can be applied to them. They define which elements on a web page should receive specific styling rules.

- Used to select HTML elements based on tag name, class, id, or attributes.
- Help apply styles like color, font, spacing, and layout.
- Make web pages structured, consistent, and visually appealing.

### Types of Selectors :
```CSS
1. Basic Selectors : Basic selectors in CSS are simple tools used for selecting by HTML element name (e.g., h1), class (.class Name), ID (#idName), or universally (* for all elements).

2. Combinator Selectors : Used to define relationships between selectors, allowing you to style elements based on their hierarchy or positioning in the document. Common combinators include descendant ( ), child (>), adjacent sibling (+), and general sibling (~).

3. Attribute Selectors : Attribute selectors in CSS target elements based on the presence or value of their attributes.

4. Pseudo-Classes : Pseudo-classes in CSS define the special states of elements for styling.

5. Pseudo-Elements : Pseudo-elements allow you to target and style specific parts of an element, such as inserting content before or after it.

- They can be used to style parts of text, like the first letter or line of a paragraph.
- Pseudo-elements are commonly used to enhance and beautify the internal content of elements.
```

### Explanation :
<i>

Basic Selectors
```CSS
1. Universal Selector (*) : Selects all elements on the page and applies the same style universally.

2. Element Selector: Targets all elements of a specific type, such as paragraphs or headers.

3. Class Selector (.): Applies styles to elements with a specific class attribute.

4. ID Selector (#): Styles a single element identified by its unique id.
```

Combinator Selectors
```CSS
1. Descendant Selectors : Targets an element inside another, such as paragraphs inside div.

2. Child Selector (>) : They only affects the direct child elements of a parent.

3. Adjacent Sibling Selector (+): Styles an element immediately following another.

4. General Sibling Selector (~) : Styles all siblings that follow a specific element.
```

Attribute Selectors
```CSS
1. Presence Selector: It selects elements that contain a specific attribute.

2. Attribute Value Selector: It targets elements with a particular attribute value.

3. Substring Matching(^=): It matches elements where the attribute contains a substring.

4. Wildcard Selector (*=): Matches elements where the attribute value contains a specific string.

5. Ends With Selector ($=): Matches elements whose attribute value ends with a specific string.

6. Word Match Selector (~=): Matches elements whose attribute contains a specific whole word (space-separated).

7. Hyphen Match Selector (|=): Matches elements whose attribute value starts with a word followed by a hyphen.
```

Pseudo-Classes
```CSS
1. :hover: Styles elements when the user hovers over them.

2. :focus: Styles the elements when the user focus on any particular element.

3. :first-child: Styles the element which is the first child of it's parent.

4. :last-child: Style's the element which is the last child of it's parent.

5. :not: Helps to remove a particular element from the styling index or styling context.
```

Pseudo-Elements
```CSS
1. ::before: To insert some content before an element.

2. ::after: To insert some content after an element.

3. ::first-line: Styles the first line of text within a block element. Line breaks mark the beginning of a new line.

4. ::first-letter: It Styles the first-letter of a word or a sentence.

5. ::placeholder: Styles the placeholder of a specific input field.
```

### Example : 
1. Basic Selector

`Universal Selector (*)`
```CSS
<html>
<head>
    <style>
        * {
            color: red;
        }
    </style>
</head>
<body>
    <h1>Header Text</h1>
    <p>Paragraph Text</p>
</body>
</html>
```

`Element Selector`
```CSS
<html>
<head>
    <style>
        p {
            font-size: 16px;
        }
    </style>
</head>
<body>
    <p>This paragraph styled with font size 16px.</p>
</body>
</html>
```

`Class Selector (.)`
```CSS
<html>
<head>
    <style>
        .button {
            background-color: blue;
            color: white;
        }
    </style>
</head>
<body>
    <button class="button">Click Me!</button>
</body>
</html>
```
`ID Selector (#)`
```CSS
<html>
<head>
    <style>
        #header {
            background-color: gray;
        }
    </style>
</head>
<body>
    <div id="header">This is the header section.</div>
</body>
</html>
```

2. Combinator Selectors

`Descendant Selectors`
```CSS
<html>
<head>
    <style>
        div p {
            color: red;
        }
    </style>
</head>
<body>
    <div>
        <p>This paragraph inside a div will be red.</p>
    </div>
</body>
</html>
```

`Child Selector (>)`
```CSS
<html>
<head>
    <style>
        div>p {
            margin-left: 20px;
        }
    </style>
</head>
<body>
    <div>
        <p>This is a direct child and has a left margin.</p>
        <div>
            <p>This is not a direct child.</p>
        </div>
    </div>
</body>
</html>
```

`Adjacent Sibling Selector (+)`
```CSS
<html>
<head>
    <style>
        h1+p {
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>This is a header.</h1>
    <p>This is immediately following the header and is bold.</p>
    <p>This will not be bold.</p>
</body>
</html>
```

`General Sibling Selector (~)`
```CSS
<html>
<head>
    <style>
        h1~p {
            font-style: italic;
        }
    </style>
</head>
<body>
    <h1>This is a header.</h1>
    <p>This is a sibling of the header and will be italicized.</p>
    <p>This will also be italicized because it's a sibling of the header.</p>
</body>
</html>
```

3. Attribute Selectors

`Presence Selector`
```CSS
<html>
<head>
    <style>
        input[type] {
            border: 2px solid black;
        }
    </style>
</head>
<body>
    <input type="text" placeholder="Text input">
    <input type="number" placeholder="Number input">
</body>
</html>
```

`Attribute Value Selector`
```CSS
<html>
<head>
    <style>
        input[type="text"] {
            background-color: yellow;
        }
    </style>
</head>
<body>
    <input type="text" placeholder="Text input">
    <input type="password" placeholder="Password input">
</body>
</html>
```

`Substring Matching(^=)`
```CSS
<html>
<head>
    <style>
        a[href^="https"] {
            color: green;
        }
    </style>
</head>
<body>
    <a href="https://example.com/">Secure link</a>
    <a href="http://example.com/">Non-secure link</a>
</body>
</html>
```

`Wildcard Selector (*=)`
```CSS
<html>
<head>
    <style>
        a[href*="example"] {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <a href="https://example.com/">This contains 'example' and is underlined.</a>
    <a href="https://otherlink.com">This is not underlined.</a>
</body>
</html>
```

`Ends With Selector ($=)`
```CSS
<style>
a[href$=".pdf"] {
    color: red;
}
</style>
```

`Word Match Selector (~=)`
```CSS
<style>
p[class~="highlight"] {
    background: yellow;
}
</style>
```

`Hyphen Match Selector (|=)`
```CSS
<style>
p[lang|="en"] {
    color: blue;
}
</style>
```

4. Pseudo-Classes

`:hover`
```CSS
<html>
<head>
    <style>
        a:hover {
            color: red;
        }
    </style>
</head>
<body>
    <a href="https://example.com/">Hover over this to see the effect.</a>
</body>
</html>
```

`:focus`
```CSS
<html>
<head>
    <style>
        input:focus {
            outline: 3px solid red;
        }
    </style>
</head>
<body>
    <input type="text">
</body>
</html>
```

`:first-child`
```CSS
<html><head></head>
<style>
    p:first-child {
        color: brown;
    }
</style>
<body>
    <div>
        <p>Hello1</p>
        <p>Hello2</p>
    </div>
</body></html>
```

`:last-child`
```CSS
<html><head></head>
<style>
    p:last-child {
        color:green;
    }
</style>
<body>
    <div>
        <p>Hello1</p>
        <p>Hello2</p>
    </div>
</body></html>
```

`:not`
```CSS
<html><head></head>
<style>
    p:not(.one) {
        color: blue;
    }
</style>
<body>
    <div>
        <p class="one">Hello1</p>
        <p class="two">Hello2</p>
    </div>
</body></html>
```

5. Pseudo-Elements

`::before`
```CSS
<html><head></head>
<style>
    h1::before {
        content: "★ "
    }
</style>
<body>
    <h1 tabindex="0">Welcome to Web-dev</h1>
</body></html>
```

`::after`
```CSS
<html><head></head>
<style>
    h1::after {
        content: "☀ ";
        color: orangered;
    }
</style>
<body>
    <h1 tabindex="0">Welcome to web-dev</h1>
</body></html>
```

`::first-line`
```CSS
<html><head></head>
<style>
    p::first-line {
        color: red;
    }
</style>
<body>
    <p>Welcome to web-dev<br>
        Hello dev</p>
</body>
</html>
```

`::first-letter`
```CSS
<html><head></head>
<style>
    p::first-letter {
        color: red;
        font-size: 23px;
    }
</style>
<body>
    <p>Welcome to GFG</p>
</body></html>
```

`::placeholder`
```CSS
<html><head></head>
<style>
    input::placeholder {
        font-size: 20x;
        font-family: sans-serif;
        font-weight: 900;
    }
</style>
<body>
    <input type="text" placeholder="Enter your name">
</body></html>
```
</i>

## 6. CSS Units
CSS units define the size of elements, with absolute units (like px, cm) having fixed values and relative units (like em, rem, %, vh) depending on factors like the viewport or parent elements.

### Types of Units
CSS provides two main types of units: absolute and relative.

`1. Absolute units` : Absolute units in CSS, such as px, cm, and mm, have fixed values and do not change based on the viewport or parent elements. They are used when precise, unchanging measurements are needed for elements.

```CSS
1. cm : A centimeter (cm) is a length unit in the SI system, derived from the meter (m), with 1 m = 100 cm. The SI system is maintained by the BIPM(International Bureau of Weights and Measures).

~ 1 cm = 1 / 100 m

2. mm : The millimeter (mm), introduced during the French Revolution's metric system, became part of the SI system. It is maintained by the International Bureau of Weights and Measures (BIPM).

~ 1 cm=10mm
~ 1mm=1/10 cm

3. inch(in) : The inch originated from ancient human measurements, based on the width of a thumb or the length of a dried grain of barley. It was standardized in 1959 by an international agreement, defining it as exactly 25.4 millimeters to align with the metric system.

~ 1 inch = 2.54cm =2.54 * 1cm=2.54* 10mm= 25.4mm

4. pixel (px) : A pixel (px) is the smallest unit on a digital screen, representing a point of light. More pixels mean better image clarity and higher screen resolution.

~ 1px = 0.26mm

5. pt (point) : A point (pt) is a typography unit equal to 1/72 of an inch, used for font sizes and spacing in design.

~ 1pt = 1/72 inch(1 inch=2.54cm)
~ 1pt= 1.33px

6.  pc(pica) : A pica is a unit used in print and design, equal to 12 points or 1/6 of an inch (4.233 mm). It helps define layout dimensions like font and image sizes.

~ 1pc=12pt=15.96px
```

`2. Relative Units` : Relative units in CSS are units that define sizes based on another value such as the parent element, root element, or viewport size.
<br>
They are flexible and help create responsive and adaptive layouts.

```CSS
1. em : In CSS , the "em" unit refers to the font-size of its parent element, defaulting to the root element (<html>) if it's the only one in the DOM.

2. rem : In CSS, rem is based on the font-size of the root element (<html>) and stays the same in all cases.

3. vw or view-width : In CSS, vw depends on the viewport width, which changes with screen size, so an Android phone has a smaller vw than an HD TV.

4. vh or view-height : The vh unit in CSS is 1% of the viewport height, useful for responsive design to scale elements with the window size.

5. percentage(%) : The % unit in CSS is relative to the parent element's size, allowing elements to adjust dynamically for responsive design.

6. vmin : The vmin unit in CSS is based on the smaller of the viewport's width or height, helping elements scale proportionally for responsive designs.

7. vmax : vmax is a CSS unit that represents 1% of the larger viewport dimension (width or height), helping elements scale based on the screen's dominant size.

8. ch : The ch unit in CSS represents the width of the "0" character of the current font. It's a relative unit commonly used for sizing text elements to maintain proportional widths and heights based on character dimensions.

9. ex : Relative to the height of the letter "x" in the current font, primarily used for vertical spacing and font-related measurements.

10. lh : This unit is relative and depends on the line-height of the current element.
```

### When to Use Which Unit ?
`Usecase of Absolute Units`
```CSS
1. Use for elements requiring fixed sizes, like borders, icons, or print layouts where precise measurements are important.

2. Suitable for situations where responsiveness is not a priority, such as static components.
```

`Usecase of Relative Units`
```CSS
1. Use for responsive designs that adapt to various devices and screen sizes, ensuring flexibility and accessibility.

2. Ideal for fluid layouts, scalable typography, or elements influenced by viewport or parent dimensions (e.g., vw, %, or rem).
```

### Difference Between Absolute and Relative Units in CSS
`CSS Units Comparison`

| Aspect          | Absolute Units                                                                 | Relative Units                                                                 |
|----------------|------------------------------------------------------------------------------|--------------------------------------------------------------------------------|
| Responsiveness | Not responsive; sizes remain fixed regardless of screen size or resolution.  | Highly responsive; adjust dynamically based on context.                        |
| Dependence     | Independent of parent elements or viewport size.                             | Dependent on parent, root, or viewport dimensions.                             |
| Scalability    | Harder to scale across different devices.                                    | Scales well for responsive design.                                             |
| Consistency    | Ensures exact sizing, providing uniformity across devices.                   | Size may vary based on parent or viewport, allowing flexibility.               |
| Accessibility  | Can hinder accessibility by not adjusting to user-defined browser settings.  | Adapts to user settings like font size, enhancing accessibility.               |
| Performance    | May be faster to render as values are fixed.                                 | Requires calculation based on context, potentially increasing rendering time.  |

### Example :
<i>

`1. Absolute units`

`1. cm`
```CSS
<html>
<head>
    <style>
        p {
            font-size: 2cm;
            color: green;
        }
    </style>
</head>
<body>
    <p>Welcome to web dev</p>
</body>
</html>
```

`2. mm`
```CSS
<html>
<head>
    <style>
        p {
            font-size: 20mm;
            color: green;
        }
    </style>
</head>
<body>
    <p>Welcome to web</p>
</body>

</html>
```

`3. inch(in)`
```CSS
<html>
<head>
    <style>
        p {
            font-size: .5in;
            color: green;
        }
    </style>
</head>

<body>
    <p>Welcome to web</p>
</body>
</html>
```

`4. pixel (px)`
```CSS
<html>
<head>
    <style>
        p {
            font-size: 40px;
            color: green;
        }
    </style>
</head>
<body>
    <p>Hello dev How are you?</p>
</body>
</html>
```

`5. pt (point)`
```CSS
<html>
<head>
    <style>
        p {
            font-size: 50pt;
            color: green;
        }
    </style>
</head>
<body>
    <p>Hello Jerishey</p>
</body>
</html>
```

`6. 1 pc(pica)`
```CSS
<html>
<head>
    <style>
        p {
            font-size:5pc;
            color: green;
        }
    </style>
</head>
<body>
    <p>Hello Jerishey</p>
</body>
</html>
```

`2. Relative Units`

`1. em`
```CSS
<html>
<head>
    <style>
        .ok {
            font-size: 20px;
        }
        .para {
            font-size: 2em;
        }
    </style>
</head>
<body>
    <div class="ok">
        Hello Jerishey
        <div class="para"> Hello Jerishey</div>
    </div>
</body>
</html>

# Explanation :
- The div has a font-size of 20px, and the p tag's font-size is set to 2em, where 1em equals the div's font-size.

- Therefore, the p tag's font-size is 40px (2 * 20px), based on the parent's font-size.
```

`2. rem`
```CSS
<html>
<head>
    <style>
        html {
            font-size: 25px; 
      }
.para {
            font-size: 2rem;
            color: red;
        }
    </style>
</head>
<body>
    <div class="para"> Hello Jerishey</div>
</body>
</html>

# Explanation :
- In this case, with the div set to 2rem and the root font-size at 25px, the div's font-size will be 50px (2 * 25px).
```

`3. vw or view-width`
```CSS
<html>
<head>
    <style>
        .para {
            height: 10vw;
            width: 50vw;
            border: 2px solid black;
            background-color: chocolate;
            font-size: 30px;
        }
    </style>
</head>
<body>
    <div class="para"> Hello Jerishey</div>
</body>
</html>
```

`4. vh or view-height`
```CSS
<html>
<head>
    <style>
        .full-height {
            height: 100vh;
            background-color: lightblue;
            text-align: center;
            display: flex;
            justify-content: center;
            align-items: center;
        }
    </style>
</head>
<body>
    <div class="full-height">
        <h1>This div is 100% of the viewport height (100vh)</h1>
    </div>
</body>
</html>

# Explanation :
- This code creates a div that takes up 100% of the viewport height (100vh). It centers the text inside the div both vertically and horizontally using Flexbox. The background color is light blue.
```

`5. percentage(%)`
```CSS
<html>
<head>
    <style>
        .container {
            width: 200px;
            height: 100px;
            background-color: lightgreen;
        }
        .child {
            width: 50%;
            height: 50%;
            background-color: lightcoral;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="child"></div>
    </div>
</body>
</html>

# Explanation :
- This code creates a container div with a size of 300px by 200px and a child div inside it. The child div is set to 50% of the container's width and height, with a light coral background.
```

`6. vmin`
```CSS
<html>
<head>
</head>
<style>
    div {
        height: 10vmin;
        width: 20vmin;
        background-color: blueviolet;
    }
</style>
<body>
    <div></div>
    <script>
        const vw = window.innerWidth;
        const vh = window.innerHeight;
        console.log(`Viewport width: ${vw / 100}px, Viewport height: ${vh / 100}px`);
    </script>
</body>
</html>

# Explanation :
- This code creates a div with a size of 20% of the smaller viewport dimension (vmin) and a blueviolet background. The JavaScript logs the viewport width and height in pixels to the console.
```

`7. vmax`
```CSS
<html>
<head>
    <style>
        div {
            height: 2vmax;
            width: 8vmax;
            background-color: cadetblue;
        }
    </style>
</head>
<body>
    <div>
    </div>
    <script>
        const vw = window.innerWidth;
        const vh = window.innerHeight;
        const actualvw = vw / 100;
        const actualvh = vh / 100;
        console.log("view-width:" + actualvw);
        console.log("view-height:" + actualvh);
    </script>
</body>
</html>

# Explanation :
- The code creates a div with a size of 10% of the larger viewport dimension (vmax) and a cadet blue background.

- The JavaScript calculates and logs the viewport width and height in pixels by dividing the inner Width and inner Height by 100.
```

`8. ch`
```CSS
<html>
<head>
    <style>
        .small {
            font-family: monospace;
            font-size: 25px;
            height: 10ch;
            width: 10ch;
            background-color: cornflowerblue;
        }
    </style>
</head>
<body>
    <div class="small">
        Hello Jerishey
    </div>
</body>
</html>

# Explanation :
- In this code we have created a div with the class name of small and the height and width of the small box has been set up to 10 times the height of the 'x' character in the current font which is the monospace font.
```

`9. ex`
```CSS
<html>
<head>
    <style>
        .small {
            font-family: monospace;
            font-size: 25px;
            height: 10ex;
            width: 10ex;
            background-color: cornflowerblue;
        }

    </style>
</head>
<body>
    <div class="small">
        Hello Jerishey
    </div>
</body>
</html>

# Explanation :
- The code creates a div with the class .small, displaying the text "Hello Jerishey" in a monospace font with a font size of 25px.

- The div 's height and width are set to 10ex, where "ex" is based on the height of the letter "x" in the font, and the background color is cornflower blue.
```

`10. lh`
```CSS
<html>
<head>
    <style>
        .small {
            font-family: sans-serif;
            font-size: 20px;
            line-height: 8;
            height:1lh;
            width: 1lh;
            background-color: aquamarine;
        }
     
    </style>
</head>
<body>
    <div class="small">
        Hello Jerishey
    </div>
</body>
</html>

# Explanation :
- The code creates a div with the class .small, displaying "Hello Jerishey" with a sans-serif font, 25px font size, and a line height of 10. The div's height and width are set using the lh unit, based on the line height.

- Since the line height is 10, the div's height and width are both 20px (2 * line height), and the background color is aquamarine.
```
</i>

## 7. CSS Display Property
The CSS display property determines how an element is displayed on a webpage, defining its layout behavior and how it interacts with other elements.

- It specifies the type of rendering box an element generates.
- Controls whether an element is shown as a block, inline, flex, grid, etc.
- Affects the layout structure and overall page flow.

### Understanding the Display Property
The display property defines how an HTML element should be displayed. It controls the box type generated by an element, affecting its positioning and behavior within the document flow.

```CSS
1. block : Displays the element as a block-level element that takes full available width, always starts on a new line, and allows setting width, height, margin, and padding.

Uses:
- Used to create sections like headers, paragraphs, and div layouts
- Helps structure content vertically on a webpage

2. inline : Displays the element inline within text flow, only taking the required width, and does not start on a new line. Width and height cannot be applied properly.

Uses:
- Used for text elements like links and spans
- Helps keep elements in a single line

3. inline-block : Combines features of inline and block, meaning the element stays in line but also allows width, height, margin, and padding to be applied.

Uses:
- Used for buttons and images with controlled size
- Helps align elements horizontally with spacing

4. None : Completely removes the element from the document flow, meaning it is not visible and occupies no space, unlike visibility: hidden.

Uses:
- Used for buttons and images with controlled size
- Helps align elements horizontally with spacing

5. flex : Defines a flex container that enables flexible layout, allowing child elements to be aligned, spaced, and resized dynamically in one direction (row or column).

Uses:
- Used to build responsive layouts
- Helps align items (center, space-between, etc.) easily

6. grid : Defines a grid container that allows layout in two dimensions (rows and columns), making it easy to create complex and responsive designs.

Uses:
- Used for complex layouts with rows and columns
- Helps design responsive web pages
```

### Example:
```CSS
<!DOCTYPE html>
<html>
<head>
  <title>Display Property Example</title>

  <style>
    /* 1. BLOCK */
    .block {
      display: block;
      background-color: lightblue;
      margin: 10px 0;
      padding: 10px;
    }

    /* 2. INLINE */
    .inline {
      display: inline;
      background-color: yellow;
    }

    /* 3. INLINE-BLOCK */
    .inline-block {
      display: inline-block;
      width: 120px;
      height: 50px;
      background-color: orange;
      margin: 5px;
      text-align: center;
      line-height: 50px;
    }

    /* 4. NONE */
    .hidden {
      display: none;
    }

    /* 5. FLEX */
    .flex-container {
      display: flex;
      justify-content: space-between;
      background-color: lightgreen;
      padding: 10px;
    }

    .flex-item {
      background-color: green;
      color: white;
      padding: 10px;
    }

    /* 6. GRID */
    .grid-container {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      background-color: lightgray;
      padding: 10px;
    }

    .grid-item {
      background-color: gray;
      color: white;
      padding: 20px;
      text-align: center;
    }
  </style>

</head>
<body>

  <!-- BLOCK -->
  <div class="block">Block Element 1</div>
  <div class="block">Block Element 2</div>

  <!-- INLINE -->
  <span class="inline">Inline 1</span>
  <span class="inline">Inline 2</span>

  <br><br>

  <!-- INLINE-BLOCK -->
  <div class="inline-block">Box 1</div>
  <div class="inline-block">Box 2</div>

  <!-- NONE -->
  <p class="hidden">You can't see me (display: none)</p>

  <!-- FLEX -->
  <div class="flex-container">
    <div class="flex-item">Flex 1</div>
    <div class="flex-item">Flex 2</div>
    <div class="flex-item">Flex 3</div>
  </div>

  <br>

  <!-- GRID -->
  <div class="grid-container">
    <div class="grid-item">Grid 1</div>
    <div class="grid-item">Grid 2</div>
    <div class="grid-item">Grid 3</div>
  </div>

</body>
</html>
```

## 8. CSS Flexbox
The Flexible Box Layout module introduces a one-dimensional layout system that handles space distribution and item alignment effectively. It works seamlessly for horizontal (row) or vertical (column) arrangements, making it a go-to solution for responsive designs.

### Features :
```CSS
1. Flexbox eliminates the need for floats or complex positioning, enabling responsive and dynamic layouts.

2. It aligns items efficiently, distributing space within a container, even when their sizes are dynamic or unknown.

3. Flexbox is supported in all modern browsers, making it a reliable choice for creating flexible designs.
```

### Flexbox :

`1. Flexbox Components :`
```CSS
- Flex Container: The parent div containing various divisions.
- Flex Items: The items inside the container div.
```

`2. Flexbox Axes :` Flexbox operates on two axes:
```CSS
1. Main Axis:
- Main Start: The start of the main axis.
- Main Size: The length between Main Start and Main End.
- Main End: The endpoint of the main axis.

2. Cross Axis: The cross axis will be perpendicular to the main axis.
- Cross Start: The start of the cross axis.
- Cross Size: The length between Cross Start and Cross End.
- Cross End: The endpoint of the cross axis.

3. Flex Direction Properties
- Left to Right: flex-direction: row;
- Right to Left: flex-direction: row-reverse;
- Top to Bottom: flex-direction: column;
- Bottom to Top: flex-direction: column-reverse;

4. Aligning and Justifying Content:
- justify-content: Aligns items along the main axis (e.g., flex-start, flex-end, center, space-between, space-around).
- align-items: Aligns items along the cross axis (e.g., stretch, center, flex-start, flex-end).
- align-content: Aligns rows within a flex container when there is extra space on the cross axis. 
```

## 9. CSS Grid 
The CSS Grid Layout Module is a powerful two-dimensional layout system that enables the creation of complex and responsive designs. It allows precise control over rows, columns, and the positioning of elements.

### Features:
```CSS
1. Grid layouts work with both rows and columns simultaneously.

2. It helps create structured and responsive page layouts.

3. Elements can be positioned precisely using grid lines and areas.
```

<b> Syntax : </b>
```CSS
.class {    display: grid;}
```

### CSS Grid Properties :
```CSS
### CSS Grid Properties :

1. column-gap : Defines the space between columns in a grid or multi-column layout.

2. gap : Sets spacing between rows and columns (shorthand for row-gap and column-gap).

3. grid : A layout system that creates rows and columns for designing web pages without floats.

4. grid-area : Specifies the position and size of a grid item using row and column lines.

5. grid-auto-columns : Defines the size of automatically created columns.

6. grid-auto-flow : Controls how auto-placed items flow in the grid (row, column, dense).

7. grid-auto-rows : Sets the height of automatically generated rows.

8. grid-column : Shorthand to define start and end position of a column.

9. grid-column-end : Specifies where the grid item will end in the column direction.

10. grid-column-gap : Sets the space between columns (older property, replaced by column-gap).

11. grid-column-start : Specifies where the grid item starts in the column direction.

12. grid-gap : Shorthand for row-gap and column-gap (older version of gap).

13. grid-row : Shorthand to define start and end position of a row.

14. grid-row-end : Defines where the grid item ends in the row direction.

15. grid-row-gap : Sets the space between rows (older property, replaced by row-gap).

16. grid-row-start : Defines where the grid item starts in the row direction.

17. grid-template : Shorthand for defining rows, columns, and areas in one line.

18. grid-template-areas : Defines named areas for layout design.

19. grid-template-columns : Defines the number and size of columns in the grid.

20. grid-template-rows : Defines the number and height of rows in the grid.
```

### Example :
```CSS
<!DOCTYPE html>
<html>
<head>
  <title>Grid Example</title>

  <style>
    .container {
      display: grid; /* grid */

      grid-template-columns: repeat(3, 1fr); /* columns */
      grid-template-rows: auto auto; /* rows */

      gap: 10px; /* gap */
      column-gap: 20px; /* column-gap */

      grid-auto-rows: 100px; /* auto rows */
      grid-auto-columns: 50px; /* auto columns */

      grid-auto-flow: row; /* flow */

      background-color: lightgray;
      padding: 10px;
    }

    .item1 {
      grid-column: 1 / 3; /* span columns */
      grid-row: 1 / 2; /* row position */
      background-color: coral;
    }

    .item2 {
      grid-column-start: 3; /* start column */
      grid-column-end: 4; /* end column */
      background-color: lightblue;
    }

    .item3 {
      grid-row-start: 2; /* start row */
      grid-row-end: 3; /* end row */
      background-color: lightgreen;
    }

    .item4 {
      grid-area: 2 / 2 / 3 / 4; /* grid-area */
      background-color: orange;
    }

    .item {
      padding: 20px;
      text-align: center;
      color: white;
    }
  </style>

</head>
<body>

  <div class="container">
    <div class="item item1">Item 1</div>
    <div class="item item2">Item 2</div>
    <div class="item item3">Item 3</div>
    <div class="item item4">Item 4</div>
  </div>

</body>
</html>
```

### Best Practices for CSS Grid Layout
```CSS
1. Use Flexible Units: Utilize flexible units like fr and minmax() to create responsive layouts that adapt to various screen sizes.

2. Define Explicit Grid Areas: Clearly specify grid areas using grid-template-areas for better readability and maintainability of your code.

3. Combine with Other Layout Methods: Integrate CSS Grid with Flexbox to leverage the strengths of both and achieve complex, responsive design.
```

## 10. CSS Background
The CSS background is the area behind an element's content, which can be a color, image, or both. The background property lets you control these aspects, including color, image, position, and repetition.

### CSS Background Property
`1. Background color Property :` The background-color property in CSS sets the background color of an element. It can accept a color name (e.g., "red"), HEX value (e.g., "#ff0000"), or RGB value (e.g., "rgb(255, 0, 0)").

<b> Syntax : </b>
```CSS
element {
    background-color : color | transparent| initial | inherit;
}
```
`CSS background-color Property Values`
```CSS
1. color Value: It defines the background color value or color codes. For example: A color name can be given as: “green” or HEX value as “#5570f0” or RGB value as “rgb(25, 255, 2)”.

2. transparent Value: It is the default value. It specifies the transparent background-color.

3. initial Value: It is used to set the default value. It does not set the background color.

4. Inherit: The inherit keyword for the color property causes an element to take the color value from its parent element. This means the text, borders, backgrounds, or other elements within the element will automatically inherit the color of their parent.
```

`2. Background Image Property :` The background-image property in CSS is used to set an image as the background of an element. By default, the image is repeated to cover the entire element unless specified otherwise.

<b>Syntax : </b>
```CSS
body {
    background-image : url("image.jpg");
}
```

`3. CSS background-repeat Property :` The background-repeat property in CSS is used to repeat the background image both horizontally and vertically. It also decides whether the background-image will be repeated or not.

<b>Syntax : </b>
```CSS
background-repeat: repeat|repeat-x|round|space|repeat-y|no-repeat|initial|
inherit;
```
`Property Values:`
```CSS
- repeat: This property is used to repeat the background image both horizontally and vertically. The last image will be clipped if it is not fit in the browser window. 

- repeat-x: This property is used to repeat the background image horizontally. 

- repeat-y: This property is used to set the background image repeated only vertically. 

- no-repeat: This property does not repeat the background image. It displays the background image only once. 
```

`4. Background-attachment Property :` The background-attachment property in CSS specifies how the background image behaves when the user scrolls the page. By setting the value to fixed, the background image stays in place while the content of the page scrolls.

<b>Syntax :</b>
```CSS
body {
    background-attachment: value;
}
```

`value`
```CSS
1. scroll (default) : Background scrolls along with the page.

2. fixed : Background stays fixed in place while content scrolls.

3. local : Background scrolls along with the element’s content.
```

`5. CSS background-position Property :` The CSS background-position property sets the starting position of a background image within an element. It allows you to use keywords, percentages, or length values to control where the image is placed.

<b>Syntax :</b>
```CSS
element {
    background-position: value;
}
```

`CSS Background Position Values`
```CSS
1. background-position: left top;
Definition: Positions the background image at the top-left corner of the element (0% from left, 0% from top).

2. background-position: left center;
Definition: Aligns the background image at the center-left (0% horizontally, 50% vertically).

3. background-position: left bottom;
Definition: Places the background image at the bottom-left corner (0% from left, 100% from top).

4. background-position: center top;
Definition: Positions the background image at the top-center (50% horizontally, 0% vertically).

5. background-position: center center;
Definition: Centers the background image both horizontally and vertically (50%, 50%).

6. background-position: center bottom;
Definition: Aligns the background image at the bottom-center (50% horizontally, 100% vertically).

7. background-position: right top;
Definition: Positions the background image at the top-right corner (100% from left, 0% from top).

8. background-position: right center;
Definition: Aligns the background image at the center-right (100% horizontally, 50% vertically).

9. background-position: right bottom;
Definition: Places the background image at the bottom-right corner (100% from left, 100% from top).

10. background-position: 25% 75%;
Definition: Positions the image 25% from the left and 75% from the top of the element.

11. background-position: 30px 80px;
Definition: Positions the image 30 pixels from the left and 80 pixels from the top of the element.
```

### Example :
```CSS
<!DOCTYPE html>
<html>
<head>
  <style>
    body {
      background-color: lightblue;                 /* Background color */
      background-image: url("bg.jpg");             /* Background image */
      background-repeat: no-repeat;                /* No repeat */
      background-position: center;                 /* Center position */
      background-size: cover;                      /* Cover full screen */
      background-attachment: fixed;                /* Fixed background */
    }
  </style>
</head>
<body>

  <h1>Hello World</h1>
  <p>This page uses CSS background properties.</p>

</body>
</html>
```

## 11. CSS Borders
CSS borders define the outline around an HTML element, providing visual separation and emphasis within a webpage layout.

### Features :
```CSS
- Width is determined by the thickness of the border.
- Style is defined by the appearance of the border (solid, dashed, dotted, etc.).
- Color is specified by the chosen hue of the border.
- Borders can be applied to all sides or specific edges of an element.
```
<b>Syntax :</b>
```CSS
element {
    border: 1px solid black;
} 
```

### CSS Border Properties
`1. CSS border-style Property :` CSS border-style Property is used to set the border style, and it is a shorthand property that sets the line style for all four sides of an element's border.

<b>Syntax :</b>
```CSS
border-style: value;
```

`CSS border-style Property Values:`
```CSS
- none: No border is created and it is left plain.
- hidden: Just like none, it doesn't show any border unless a background image is added, then the border-top-width will be set to 0 irrespective of the user-defined value.
- dotted: A series of dots are displayed in a line as the border.
- solid: A single solid and bold line is used as a border.
- dashed: A series of square dashed lines are used as a border.
- double: Two lines placed parallel to each other act as the border.
- groove: Displays a 3D grooved border, its effect depends on border-color value.
- ridge: Displays a 3D ridged border, its effect depends on border-color value.
- inset: displays a 3D inset border, its effect depends on border-color value.
- outset: Displays a 3D outset border, its effect depends on border-color value.
```

`2. CSS border-width Property :` The border-width property in CSS sets the width of an element’s border. You can specify a single width for all four sides or define different widths for each side (top, right, bottom, and left).

<b>Syntax :</b>
```CSS
border-width: length | thin | medium | thick | initial | inherit
```
`Property values :`
```CSS
1. length : Specifies the border thickness using fixed units like px, em, rem, etc., allowing precise control over border size.

2. thin : Sets the border to a thin width, which is a predefined value determined by the browser.

3. medium : Sets the border to a medium thickness and is the default border width value.

4. thick : Sets the border to a thick width, larger than medium, based on browser-defined size.

5. initial : Resets the border width to its default value, which is medium.

6. inherit : Inherits the border width from its parent element, maintaining consistency in styling.
```

`3. CSS border-color Property :` The CSS border-color property allows developers to define the color of an element's border, enhancing the visual design of a webpage. It works in conjunction with the border property to provide control over the appearance of borders using various color values like-named colors, hex codes, or RGB values.

<b>Syntax :</b>
```CSS
border-color: color-value;

Multiple Sides Syntax ->
border-color: top-color right-color bottom-color left-color;
```
`Property Values for border-color`
```CSS
1. color : Specifies the border color using color names, HEX, RGB, or HSL values.

2. transparent : Makes the border color transparent (invisible but space is still there).

3. initial : Sets the border color to its default value.

4. inherit : Inherits the border color from the parent element.
```

`4. CSS border-radius Property :` The CSS border-radius property allows you to round the corners of an element’s outer border, giving it a smooth, curved appearance. You can specify one, two, three, or four values to individually control the radius of each corner.

<b>Syntax :</b>
```CSS
border-radius: 1-4 length|% / 1-4 length|%|initial|inherit;
```

`Property Values`
```CSS
1. length : Specifies the radius of the corners using units like px, em, rem, etc.

2. percentage (%) : Defines the radius as a percentage of the element’s size, often used to create circles or ellipses.

3. initial : Sets the border radius to its default value (0, meaning no rounding).

4. inherit : Inherits the border radius value from the parent element.
```

### Example :
```CSS
<!DOCTYPE html>
<html>
<head>
  <style>
    .box {
      width: 300px;
      padding: 20px;
      margin: 20px;

      /* Border width */
      border-width: 5px;

      /* Border style */
      border-style: solid;

      /* Border color */
      border-color: red;

      /* Individual sides */
      border-top: 5px dashed blue;
      border-right: 5px solid green;
      border-bottom: 5px dotted orange;
      border-left: 5px double purple;

      /* Border radius */
      border-radius: 15px;

      /* Individual corner radius */
      border-top-left-radius: 20px;
      border-bottom-right-radius: 30px;
    }
  </style>
</head>
<body>

  <div class="box">
    This box demonstrates all CSS border properties.
  </div>

</body>
</html>
```

### Use Cases of CSS Borders
```CSS
1. Styling Buttons : Borders enhance button designs, making them more visually appealing and clickable.

2. Creating Dividers : Borders can act as separators between content sections, providing clear visual breaks.

3. Customizing Images : Apply borders around images to frame them, making thumbnails stand out.

4. Designing Navigation Menus : Borders can define the boundaries of navigation links or items.
```
## 12. CSS Fonts
CSS fonts are used to style and enhance the appearance of text on a webpage, making it more readable and visually appealing. They help control how text looks and fits within the overall design.


### Features :
```CSS
1. Used to set the size, weight, style, and color of text.

2. Help create a consistent and attractive look across a website.

3. Improve readability and align the text style with the website’s theme.

Example:
<html>
<head>
    <style>
        .gfg {
            font-family: "Arial, Helvetica, sans-serif";
            font-size: 60px;
            color: #090;
            text-align: center;
        }
    </style>
</head>

<body>
    <div class="gfg">CSS</div>
</body>

</html>

- The code applies a green, 60px Arial font to the text "CSS" and centers it on the page.

- The text is styled using the .gfg class in the HTML.
```

### How to Apply Fonts in CSS
Fonts in CSS are applied using specific properties that control the style and appearance of text.

`1. font-family :` The font-family property defines which font(s) should be used for text. You can provide a list of fonts as a fallback mechanism in case the preferred font is unavailable.
```CSS
Syntax : 
- font-family: "Font Name", generic-font-name; 

Example:
body {
    font-family: "Arial", sans-serif;
}
```

`2. font-size :` The font-size property controls the size of the text. You can set the size in several units, including pixels (px), ems (em), and percentages (%).
```CSS
Syntax:
- font-size: value;

Example:
h1 {
    font-size: 32px; /* Pixels */
}

p {
    font-size: 1.2em; /* Relative to the parent element */
}

- Pixels (px) provide a fixed font size.
- Ems (em) are relative to the parent element’s font size, making them useful for responsive design.
```

`3. font-weight :` The font-weight property controls the thickness of the text. It can accept values like normal, bold, or numeric values (100 to 900).
```CSS
Syntax:

- font-weight: value;

Example:
p {
    font-weight: bold; /* Bold text */
}

strong {
    font-weight: 700; /* Equivalent to bold */
}

- 
Numeric values allow for finer control over weight (e.g., 100 for light, 900 for extra bold).
```
`4. font-style :` The font-style property defines the style of the font, typically italic or normal.
```CSS
Syntax:

- font-style: value;

Example:
em {
    font-style: italic; /* Italicized text */
}

p {
    font-style: normal; /* Normal text */
}
```

`5. line-height :` The line-height property defines the space between lines of text. Increasing line height improves readability, especially for long paragraphs.
```CSS
Syntax:

- line-height: value;

Example:
p {
    line-height: 1.5; /* 1.5 times the font size */
}
```

### Web Safe Fonts Vs Custom Fonts
This comparison highlights the difference between universally supported system fonts (web-safe) and designer-selected custom fonts used for unique web styling.

`1. Web Safe Fonts :` Web safe fonts are commonly supported across all browsers and operating systems. These fonts are pre-installed on most computers, ensuring your text appears the same across devices.
<i>
```CSS
Common Web Safe Fonts

1. Arial
2. Times New Roman
3. Courier New
4. Verdana
5. Georgia

Example:
body {
    font-family: "Verdana", sans-serif;
}
```
</i>

`2. Custom Fonts :` Custom fonts allow you to use fonts that are not pre-installed on a user’s device. You can load them using web fonts. The most popular method for using custom fonts is through Google Fonts, or by hosting fonts on your own server.
<i>
```CSS
<head>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <h1 style="font-family: 'Roboto', sans-serif;">Hello, World!</h1>
</body>
```

### Properties of CSS Fonts
To customize fonts effectively in web design, it’s crucial to understand the main CSS font properties:
```CSS
- font-family: Specifies the font type.
- font-size: Determines the size of the text.
- font-weight: Adjusts the thickness of the text.
- font-style: Controls the slant of the text (e.g., italic).
- line-height: Sets the space between lines of text.
- letter-spacing: Modifies the space between characters.
- text-transform: Controls the capitalization of text.
```
</i>

## 13. CSS Colors
CSS colors are used to change the look of text, backgrounds, borders, and other elements on a webpage. They help make a site more attractive and easy to read.

```CSS
1. Colors can be set using names, HEX codes, RGB, RGBA, HSL, or HSLA values.

2. Used to style text, backgrounds, and borders.

3. Help create contrast, highlight content, and improve visual design.
```

### Use Cases of CSS Colors
CSS colors play a vital role in the design and functionality of a webpage.

`1. Background Colors :` You can use background-color to set the color of an element’s background. It's typically used for sections, divs, headers, footers, etc.
```CSS
<html>
<head>
    <style>
        .bg-example {
            background-color: #FF5733; /* Red-Orange background */
            padding: 20px;
            color: white;
        }
    </style>
</head>
<body>
    <div class="bg-example">This div has a warm background color!</div>
</body>
</html>
```

`2. Text Colors :` The color property is used to apply color to the text. It's important to ensure good contrast between the text and the background for readability.
```CSS
<html>
<head>
    <style>
        .text-example {
            color: rgb(255, 0, 0); /* Red text */
            font-size: 20px;
        }
    </style>
</head>
<body>
    <p class="text-example">This text is in red.</p>
</body>
</html>
```

`3. Border Colors :` You can use the border property to apply color to an element's border. It's commonly used for buttons, cards, or form inputs to create visible outlines.
```CSS
<html>
<head>
    <style>
        .border-example {
            border: 5px solid rgba(0, 255, 0, 0.5); /* Semi-transparent green border */
            padding: 10px;
            margin: 10px;
        }
    </style>
</head>
<body>
    <div class="border-example">This div has a semi-transparent green border.</div>
</body>
</html>
```

`4. Hover Effects :` Use the :hover pseudo-class to change the color of an element when a user hovers over it, adding interactivity to your design.
```CSS
<html>
<head>
    <style>
        .hover-example {
            background-color: #4CAF50; /* Green background */
            color: white;
            padding: 20px;
            text-align: center;
            cursor: pointer;
        }

        .hover-example:hover {
            background-color: #45a049; /* Darker green on hover */
        }
    </style>
</head>
<body>
    <div class="hover-example">Hover over me to change the background color!</div>
</body>
</html>
```

`5. Shadows and Text Effects :` You can use box-shadow to add shadows around elements or text-shadow for adding shadows to the text, creating depth and emphasis.
```CSS
<html>
<head>
    <style>
        .shadow-example {
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); 
            color: #FF5733;
            font-size: 30px;
        }

        .box-shadow-example {
            box-shadow: 3px 3px 15px rgba(0, 0, 0, 0.3);
            padding: 20px;
            background-color: #FFF;
        }
    </style>
</head>
<body>
    <p class="shadow-example">This text has a shadow effect.</p>
    <div class="box-shadow-example">This div has a box shadow.</div>
</body>
</html>
```

`6. Gradients :` CSS allows you to create gradients using the background property. Gradients can transition smoothly between two or more colors.
```CSS
<html>
<head>
    <style>
        .gradient-example {
            background: linear-gradient(to right, #FF5733, #33FF57);
            padding: 40px;
            color: white;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="gradient-example">This div has a linear gradient background.</div>
</body>
</html>
```

### Example:
```CSS
<html>
<head>
    <style>
        .hex-example {
            background-color: #FF5733; /* Hexadecimal color */
        }
        .rgb-example {
            color: rgb(255, 0, 0); /* RGB color */
        }
        .rgba-example {
            color: rgba(0, 255, 0, 0.5); /* RGBA color with transparency */
        }
        .hsl-example {
            color: hsl(120, 100%, 50%); /* HSL color */
        }
        .hsla-example {
            color: hsla(120, 100%, 50%, 0.3); /* HSLA color with transparency */
        }
    </style>
</head>
<body>
    <div class="hex-example">This div has a Hexadecimal background color.</div>
    <div class="rgb-example">This text is in RGB red.</div>
    <div class="rgba-example">This text is in RGBA green with 50% transparency.</div>
    <div class="hsl-example">This text is in HSL green.</div>
    <div class="hsla-example">This text is in HSLA green with 30% opacity.</div>
</body>
</html>
```

`Explanation:`
<i>
```CSS
1. Background Color (background-color): #FF5733; adds a bright red-orange background, and padding: 20px; provides inner spacing.

2. Text Color (color): rgb(255, 0, 0); sets the text to red, and font-size: 20px; makes it larger.

3. Border Color (border): 5px solid rgba(0, 255, 0, 0.5); adds a semi-transparent green border with padding: 10px; and margin: 10px; for spacing.

4. Hover Effects: background-color: hsl(120, 100%, 50%); gives a bright green background that changes to a lighter transparent green on hover.
```
</i>

## 14. CSS Margins
CSS margins are used to create space outside an element’s border, helping to separate it from other elements on a webpage. They help in organizing the layout and preventing content from appearing too close together.

```CSS
Syntax:

body {  margin: value;}
```
### Types of Margin Values
```CSS
1. Pixels (px): The most common unit, specifies a fixed number of pixels.

2. Percentage (%): The margin is calculated as a percentage of the containing. element's width (for horizontal margins) or height (for vertical margins).

3. Other units: Less common units like em, rem, vh, and vw can also be used for relative sizing.

4. Auto: The browser calculates a suitable margin size, often used for centering elements.
```

### Margin Properties Values

| **Margin Property** | **Description**                                      | **Example**          |
| ------------------- | ---------------------------------------------------- | -------------------- |
| margin-top          | Sets the top margin of an element.                   | margin-top: 20px;    |
| margin-right        | Sets the right margin of an element.                 | margin-right: 15px;  |
| margin-bottom       | Specifies the margin at the bottom of an element.    | margin-bottom: 30px; |
| margin-left         | Determines the width of the margin on the left side. | margin-left: 10px;   |
| margin              | Shorthand to set margins on all four sides.          | margin: 10px 20px;   |

### Example:
```CSS
<!DOCTYPE html>
<html>
<head>
  <style>
    div {
      background-color: lightblue;
      margin: 20px 40px; /* top-bottom: 20px, left-right: 40px */
      padding: 10px;
    }
  </style>
</head>
<body>

  <div>
    This box has margin applied around it.
  </div>

</body>
</html>
```

## 15. CSS Padding
CSS Padding property is used to create space between the element's content and the element's border. It only affects the content inside the element.

### Features:
```CSS
CSS padding is different from CSS margin as the margin is the space between adjacent element borders and padding is the space between content and element's border.
We can independently change the top, bottom, left, and right padding using padding properties.
```
### CSS padding properties
CSS provides properties to specify padding for individual sides of an element which are defined as follows:
```CSS
1. Padding: The overall space inside an element can be set using padding, which applies to all four sides at once.

2. Padding-top: The space on the top side of an element is set using padding-top.

3. Padding-right: The space on the right side of an element is controlled by padding-right.

4. Padding-bottom: The space at the bottom of an element is determined using padding-bottom.

5. Padding-left: The space on the left side of an element is set using padding-left.

6. Padding properties can have the following padding values:
- Length: in cm, px, pt, etc.
- Width: % width of the element.
- inherit: inherit padding from the parent element.
```

### Shorthand Property for Padding in CSS
The Shorthand Padding Property in CSS allows you to set the padding on all sides (top, right, bottom, left) of an element in a single line with some combinations, so we can easily apply padding to our targeted element.

```CSS
There are four cases while using shorthand property:

1. If the padding property has one value.
2. If the padding property contains two values.
3. If the padding property contains three values.
4. If the padding property contains four values.
```
`1. CSS Shorthand Padding Property for One Value :` f the padding property has one value, then it applies padding to all sides of an element.

<b>Example:</b>
```CSS
<!DOCTYPE html>
<html>

<head>
    <title>Padding Property has One Value</title>
    <style>
        body {
            margin: 0;
            padding: 20px;

        }

        h2 {
            color: green;
        }

        .myDiv {
            background-color: gray;
            border: 2px solid black;
            text-align: center;
            width: 40%;

            /* Applies 10px padding to all sides */
            padding: 20px;
        }

        .inner {
            height: 70px;
            width: 70px;
            background-color: pink;
            display: flex;
            align-items: center;
            justify-content: center;
        }
    </style>
</head>

<body>
    <div class="myDiv">
        <div class="inner">Padding</div>
    </div>
</body>

</html>
```

`2. Padding Property for Two Values :` If the padding property contains two values, then the first value applies to the top and bottom padding, and the second value applies to the right and left padding.

<b>Example: </b>
```CSS
<!DOCTYPE html>
<html>

<head>
    <title>Padding Property Contains Two Value</title>

    <style>
        body {
            margin: 0;
            padding: 20px;

        }

        h2 {
            color: green;
        }

        .myDiv {
            background-color: gray;
            border: 2px solid black;
            text-align: center;
            width: 40%;

            padding: 10px 20px;
            /* Applies 10px padding to top and bottom, 
               20px padding to right and left */
        }

        .inner {
            height: 70px;
            width: 70px;
            background-color: pink;

        }
    </style>
</head>

<body>
    <div class="myDiv">
        <div class="inner">Box</div>
    </div>
</body>

</html>
```

`3. Padding Property for Three Values :` If the padding property contains three values, then the first value sets the top padding, the second value sets the right and left padding, and the third value sets the bottom padding.

<b> Example: </b>
```CSS
<!DOCTYPE html>
<html>

<head>
    <title>Padding Property Contains Three Values</title>

    <style>
        body {
            margin: 0;
            padding: 20px;

        }

        h2 {
            color: green;
        }

        .myDiv {
            background-color: yellowgreen;
            border: 2px solid black;
            text-align: center;
            width: 40%;

            padding: 10px 20px 30px;
            /* Applies 10px padding to top, 
               20px padding to right and left, 
               30px padding to bottom */
        }

        .inner {
            height: 70px;
            width: 70px;
            background-color: grey;
        }
    </style>
</head>

<body>
    <div class="myDiv">
        <div class="inner">Box</div>
    </div>
</body>

</html>
```

`4. Padding Property Having Four Values :` If the padding property contains four values, then the first value sets the top padding, the second value sets the right padding, the third value sets the bottom padding, and the fourth value sets the left padding.

<b>Example: </b>
```CSS
<!DOCTYPE html>
<html>

<head>
    <title>Padding Property Contains Four Values</title>
    <style>
        body {
            margin: 0;
            padding: 20px;

        }

        h2 {
            color: green;
        }

        .myDiv {
            background-color: cyan;
            border: 2px solid black;
            text-align: center;
            width: 40%;

            padding: 10px 20px 15px 25px;
            /* Applies 10px padding to top, 
               20px padding to right, 
               15px padding to bottom, 
               and 25px padding to left */

        }

        .inner {
            height: 70px;
            width: 70px;
            background-color: black;
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
        }
    </style>
</head>

<body>
    <div class="myDiv">
        <div class="inner">Box</div>
    </div>
</body>

</html>
```

## 16. CSS Positioning Elements
CSS positioning is used to control the placement of elements on a web page. It allows elements to be positioned relative to the normal document flow, the browser window, or other elements.

### Features:
```CSS
The position property defines how an element is positioned.
Common position values include static, relative, absolute, fixed, and sticky.
Positioning works with properties like top, right, bottom, and left.
It helps create flexible layouts, overlays, and responsive designs.
```

`1. Static Positioning :` Static is the default position of an element. It does not accept properties like top, left, right, or bottom.

```CSS
<html>
<head>
    <style>
        div {
            border: 1px solid black;
            padding: 10px;
            margin: 10px;
        }
    </style>
</head>
<body>
    <div>Box 1</div>
    <div>Box 2</div>
</body>
</html>

- The boxes follow the normal flow of the document.
- There’s no overlap or displacement of elements.1
```

`2. Relative Positioning :` Relative positioning places an element relative to its normal position. You can move it using top, left, right, or bottom.

```bash
# HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Link CSS Example</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
    
  <div>Box 1</div>
  <div class="relative">Box 2</div>
  
</body>
</html>

# CSS
div {
            border: 1px solid black;
            padding: 10px;
            margin: 10px;
        }
.relative {
            position: relative;
            top: 20px;
            left: 30px;
        }
```

`3. Absolute Positioning :` Absolute positioning removes the element from the document flow and places it relative to the nearest ancestor with a positioning context (relative, absolute, or fixed).

```CSS
<html>
<head>
    <style>
        .container {
            position: relative;
            width: 300px;
            height: 200px;
            border: 2px solid black;
            margin: 20px auto;
        }
        .absolute {
            position: absolute;
            top: 50px;
            left: 50px;
            background-color: pink;
            padding: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <p>Container with Relative Positioning</p>
        <div class="absolute">Absolutely Positioned Element</div>
    </div>
</body>
</html>
```

`4. Fixed Positioning :` Fixed positioning removes the element from the flow and positions it relative to the viewport. It remains in place even when the page scrolls.

```CSS
<html>
<head>
    <style>
        .fixed {
            position: fixed;
            top: 10px;
            right: 10px;
            background-color: lightgreen;
            padding: 20px;
            border: 2px solid black;
        }
        .content {
            height: 1200px;
            padding: 10px;
        }
    </style>
</head>
<body>
    <h2>Fixed Positioning Example</h2>
    <div class="fixed">Fixed Box</div>
    <div class="content">
        <p>Scroll down to see that the fixed box stays in place.</p>
        <p>This content simulates a long page.</p>
    </div>
</body>
</html>
```

`5. Sticky Positioning :` Sticky positioning switches between relative and fixed based on the scroll position.

```CSS
<html>
<head>
    <style>
        .sticky {
            position: sticky;
            top: 0;
            background-color: yellow;
            padding: 10px;
        }
    </style>
</head>
<body>
    <div class="sticky">I am sticky</div>
    <p>Scroll down to see the effect.</p>
    <div style="height: 1000px;"></div>
</body>
</html>
```

## 17. CSS Overflow
CSS overflow controls how content is handled when it doesn’t fit inside an element’s box. It helps manage scrolling and visibility of extra content.

### Features:
```CSS
- Can hide, scroll, or show overflowing content.
- Common values include visible, hidden, scroll, and auto.
- Useful for keeping layouts neat and preventing content overlap.
```

<b>Synatx:</b>
```CSS
overflow: visible | hidden | scroll | auto;
```

### Property Values
The overflow property contains the following values: 
```CSS
1. visible: The content is not clipped and is visible outside the element box. 

2. hidden: The overflow is clipped and the rest of the content is invisible.

3. scroll: The overflow is clipped but a scrollbar is added to see the rest of the content. The scrollbar can be horizontal or vertical. 

4. auto: It automatically adds a scrollbar whenever it is required.

5. overflow-x and overflow-y: This property specifies how to change the overflow of elements. x deals with horizontal edges and y deals with vertical edges. 
```

<b>Example:</b>
```CSS
<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 200px;
  height: 40px;
  border: 1px solid black;
  overflow: auto;
}
</style>
</head>
<body>

<div>
  This is an example of CSS overflow. When the content inside the box is too long to fit, a scrollbar appears to let you see the rest.
</div>

</body>
</html>

Explanation:
- The overflow: auto; property adds a scrollbar when the content is larger than the box.
- The box has a fixed width and height with a black border.
- Extra text can be viewed by scrolling inside the box.
```

## 18. CSS Links
CSS Links are used to style hyperlinks and control how they appear in different states such as normal, visited, hover, and active. They help improve the look and user experience of web navigation by customizing link colors, effects, and behaviors.

### Features:
```CSS
Four states of links:

1. a:link: This is a normal, unvisited link.
2. a:visited: This is a link visited by user at least once
3. a:hover : This is a link when mouse hovers over it
4. a:active: This is a link that is just clicked.
```

<b>Syntax:</b>
```CSS
a:link {    
    color:color_name;
    }
```
### Properties of CSS Links
```CSS
1. Color : This CSS property is used to change the color of the link text. 

2. Font-family : This property is used to change the font type of a link using font-family property. 

3. Text-Decoration : This property is basically used to remove/add underlines from/to a link. 

4. background-color : This property is used to set the background color of the link. 
```

<b>Example:</b>
```CSS
<!DOCTYPE html>
<html>

<head>
    <title>Link button</title>
    <style>
        /*Setting font size for better visibility*/
        p {
            font-size: 2rem;
        }

        a {
            background-color: green;
            color: white;
            padding: 5px 5px;
            border-radius: 5px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
        }
    </style>
</head>

<body>
    <p>
        <a href="https://developer.mozilla.org/en-US/docs/Web/CSS" id="link">
            CSS
        </a>
        a Computer Science Portal for learning css.
    </p>
</body>

</html>
```
