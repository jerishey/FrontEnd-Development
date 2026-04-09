# CSS3
CSS3 is a stylesheet language that controls how HTML elements look on a website—like colors, layouts, fonts, animations, and responsiveness.

<b>Features:</b>
```CSS3
1. Advanced Selectors – Help target specific HTML elements more precisely.

2. Enhanced Colors – Allow use of modern color formats with transparency.

3. Box Model Enhancements – Add visual effects like shadows and rounded corners.

4. Animations – Enable smooth movement and style changes over time.

5. Flexbox – Provides flexible layout for aligning elements in a row or column.

6. Media Queries – Make websites responsive to different screen sizes.
```

<b>Example:</b>
```CSS3
<!DOCTYPE html>
<html>
<head>
  <title>CSS3 Flexbox Example</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: lightblue;
    }

    .box {
      width: 200px;
      height: 200px;
      background-color: blue;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 20px;
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <div class="box">
    Centered Box
  </div>

</body>
</html>

Explanation:
- Uses Flexbox (CSS3) to center the box on the screen
- Applies border-radius (rounded corners)
- Uses modern layout techniques
```

## 1. CSS Media Queries
CSS Media Queries enable web pages to adjust their layout and styles based on different screen sizes, devices, or orientations. They are essential for building responsive and adaptable web designs.

### Features:
```CSS3
1. Apply CSS rules conditionally based on screen width or height.
2. Help create responsive layouts for mobile, tablet, and desktop devices.
3. Support conditions like orientation, resolution, and device type.
4. Improve user experience across different devices.
5. Media queries apply CSS rules based on device characteristics like screen width.
```

### Media Types in CSS
```CSS3
Media Type	                    Description
all	          ->          Suitable for all media devices.
print	      ->          Used for printers.
screen	      ->          Targeted at computer screens, tablets, smartphones, etc.
speech	      ->          Designed for screen readers that read the content aloud.
```
### CSS Media Query Features
```CSS3
1. width – Applies styles based on the exact width of the viewport.
2. min-width – Applies styles when the screen width is greater than or equal to a value.
3. max-width – Applies styles when the screen width is less than or equal to a value.
4. height – Applies styles based on the viewport height.
5. orientation – Detects whether the device is in portrait or landscape mode.
6. resolution – Targets devices based on pixel density (e.g., high-resolution screens).
```

<b>Example:</b>
```CSS3
<!DOCTYPE html>
<html>
<head>
  <title>Media Query Example</title>
  <style>
    body {
      background-color: lightblue;
      font-size: 20px;
    }

    /* Media Query for small screens */
    @media (max-width: 600px) {
      body {
        background-color: lightcoral;
        font-size: 14px;
      }
    }
  </style>
</head>
<body>

  <h1>Hello World</h1>
  <p>Resize the browser window to see the effect.</p>

</body>
</html>

Explanation:
- On large screens → background is lightblue
- On small screens (≤ 600px) → background becomes lightcoral and text gets smaller
```

## 2. CSS Website Layout
A layout defines how elements are arranged on a page, ensuring that content flows logically and looks visually balanced. CSS provides flexible tools to control spacing, alignment, and responsiveness.

### Features:
```CSS3
1. Structured Sections – Divides a webpage into header, footer, sidebar, and content areas.
2. Responsive Design – Adjusts layout for different screen sizes using media queries.
3. Flexbox Layout – Aligns and distributes elements in a flexible one-dimensional layout.
4. Grid Layout – Organizes content into rows and columns for complex designs.
5. Positioning – Controls element placement using static, relative, absolute, and fixed positions.
6. Float & Clear – Helps align elements side by side (older layout method).
```

### Layout Structure
<img src="https://media.geeksforgeeks.org/wp-content/uploads/20251220122122401945/html4.webp"></img>

<i>

`1. Header (Top Section) :` The header is the topmost section of a website that usually contains the logo, website name, and sometimes a tagline.
<br>
It gives the first impression of the website and helps users identify the brand. It may also include a search bar or navigation links in some designs.
<br>
<b>Example:</b>
```CSS3
<html>
<head>
    <style>
        .header {
            background-color: green;
            padding: 15px;
            text-align: center;
        }
        .header h2 {
            color: white;
            margin: 0;
        }
    </style>
</head>
<body>
    <div class="header">
        <h2>GeeksforGeeks</h2>
    </div>
</body>
</html>

Explanation:
- The <div class="header"> element defines the header section of the webpage.
- The .header CSS class styles the header with a green background, 15 pixels of padding, and centers the text.
```

`2. Navigation (Menu) :` The navigation bar contains links to different pages of the website. It helps users move easily between sections like Home, About, Services, and Contact. It is usually placed below the header or at the top.

<b>Example:</b>
```CSS3
<html>
<head>
    <style>
        .nav_menu {
            overflow: hidden;
            background-color: #333;
        }
        .nav_menu a {
            float: left;
            display: block;
            color: white;
            text-align: center;
            padding: 14px 16px;
            text-decoration: none;
        }
        .nav_menu a:hover {
            background-color: white;
            color: green;
        }
    </style>
</head>
<body>
    <div class="nav_menu">
        <a href="#">Algo</a>
        <a href="#">DS</a>
        <a href="#">Language</a>
    </div>
</body>
</html>

Explanation:
- The .nav_menu class defines the style of the navigation menu with a dark background and ensures the links are aligned horizontally.
- The a tag inside .nav_menu defines each link's style, including white text and padding for spacing.
```

`3. Main Content :` The main content area is where the primary information of the webpage is displayed. This is the most important section because it contains the actual content users are looking for, such as articles, images, or products.

<b>Example:</b>
```CSS3
<html>
<head>
    <style>
        .columnA,
        .columnB,
        .columnC {
            text-align: center;
            color: green;
        }
    </style>
</head>
<body>
    <div class="nav_menu">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </div>

    <div class="columnA">Content for Column A</div>
    <div class="columnB">Content for Column B</div>
    <div class="columnC">Content for Column C</div>
</body>
</html>

Explanation:
- The HTML structure defines three content sections, each inside a <div>, which can be further styled or adjusted as needed for responsive layouts.
- The .columnA, .columnB, and .columnC classes style the content areas, aligning the text to the center and coloring it green.
```

`4. Sidebar :` The sidebar is a secondary section placed beside the main content. It is used to show additional information that supports the main content, such as ads, links, or recent posts. It is not the main focus but still useful.

<b>Example:</b>
```CSS3
<!DOCTYPE html>
<html>
<head>
  <title>Sidebar Example</title>
  <style>
    body {
      margin: 0;
      font-family: Arial;
    }

    .container {
      display: flex;
    }

    .content {
      width: 70%;
      padding: 20px;
      background: #f1f1f1;
    }

    .sidebar {
      width: 30%;
      padding: 20px;
      background: #ddd;
    }

    .sidebar a {
      display: block;
      margin: 10px 0;
      text-decoration: none;
      color: black;
    }
  </style>
</head>
<body>

<div class="container">
  
  <div class="content">
    <h2>Main Content</h2>
    <p>This is the main area of the website.</p>
  </div>

  <div class="sidebar">
    <h3>Sidebar</h3>
    <a href="#">Recent Posts</a>
    <a href="#">Categories</a>
    <a href="#">Advertisements</a>
  </div>

</div>

</body>
</html>

Explanation:
- Sidebar is placed beside the main content
- Uses Flexbox for layout
- Contains extra links and information
```

`5. Footer (Bottom Section) :` The footer is the bottom section of a webpage. It usually contains important information like copyright, contact details, privacy policy, and social media links. It appears on every page.

<b>Example:</b>
```CSS3
<html>
<head>
    <style>
        .footer {
            background-color: green;
            padding: 15px;
            text-align: center;
        }
    </style>
</head>
<body>
    <center style="font-size:200%; margin-bottom: 300px;">Upper section</center>
    <div class="footer">
        <a href="#">About</a><br>
        <a href="#">Career</a><br>
        <a href="#">Contact Us</a>
    </div>
</body>
</html>

Explanation:
- The .footer class defines the footer section, giving it a green background, padding, and centering the text.
- Inside the footer, there are links for "About," "Career," and "Contact Us," which provide quick access to those sections.
```
</i>

### Points to Remember
```CSS3
1. The header section contains a website logo, a search bar, and user profile information.
2. The navigation menu includes links to various categories of articles available.
3. The content section is divided into three parts (columns), with left and right sidebars containing links to other articles and advertisements. The main content section holds the current article.
4. The footer at the bottom contains the address, links, contacts, etc.
```

## 3. CSS Box Model
The CSS Box Model defines how elements are sized and positioned by assigning a box in the DOM tree that determines an element's dimensions and its position relative to other elements.

```Css
1. Content: The area where text or other content is displayed.
2. Padding: Space between the content and the element's border.
3. Border: A frame that wraps around the padding and content.
4. Margin: Space between the element's border and neighboring elements.
```

### Components of the box model
`1. Content Area :` The content area is the core part of the CSS box model that holds the actual content of an element.
```Css
1. The content area is the central part of the CSS box model, containing the main content (e.g., text, images, or elements like <p> or <span>).

2. It can be styled with CSS properties like height and width.

3. The content edge refers to the four edges of the content area.

- Left content edge
- Right content edge
- Top content edge
- Bottom content edge
```

`2. Padding Area :` The padding area is the space between an element’s content and its border, contributing to the element’s overall size and spacing.
```Css
1. The padding area is the space between the content and the border of an element.
2. It includes the areas highlighted in light green and skin color in the example.
3. The distance between the content edge and the border is the padding.
4. The border marks the end of the padding area.
6. The padding area contributes to the element's total dimensions.
7. Padding can be adjusted using CSS properties.
8. It works similarly with box-sizing: content-box and box-sizing: border-box, but with slight calculation differences.
```

`3. Border Area :` The border area is the outer boundary of an element that surrounds the padding and contributes to the element’s total height and width.
```Css
1. The area that marks the end of an element is called as the border it is the outer fencing for the element.
2. The default border properties are provided in CSS to control the thickness of this outer fencing.
3. The border area also add 's up to the complete height and width of the element.
4. The more the border width the more will be the height or width of the element.
5. In the above image the area marked with skin color is called the border area.
```

`4. Margin Area :` The margin area is the space outside an element’s border that controls the distance between the element and surrounding or parent elements.
```Css
1. The area outside the border of an element is called the margin area.
2. Basically this area depends on the parent of the element.
3. The distance between the border of the parent element and the border of the child element is called as the margin.
4. CSS has provides certain margin properties to get control over this scenario.
```

## 4. Responsive Web Design
Responsive Web Design ensures websites automatically adapt to different screen sizes, providing a smooth and user-friendly experience across all devices.

### Features:
```Css
1. Content adapts by resizing or hiding based on the device.
2. Improves user experience and reduces user drop-off.
3. Uses a single flexible layout.
4. Implemented using HTML and CSS, including HTML5 and CSS3.
```

### Benefits of Responsive Web Design
```css
1. Reduces Bounce Rate: Keeps users engaged by displaying correctly on all devices.
2. Mobile-Friendly Design: Automatically adjusts layout for smaller screens.
3. Increases Website Traffic: Allows easy access across multiple devices.
4. Enhanced User Experience: Provides a consistent and smooth experience.
5. Improved SEO Performance: Better usability helps achieve higher search rankings.
```

### Principles of Responsive Web Design
Responsive web design focuses on building websites that provide a smooth and visually appealing experience across all devices. Below are the principles to follow:
```css
1. Viewable on Multiple Devices
- Ensure the website works properly on mobiles, tablets, and desktops.
- Design layouts that adapt to different screen sizes automatically.

2. Easy to Understand
- Keep the layout clean and well-organized for better usability.
- Arrange content and features clearly to avoid user confusion.

3. Consistency
- Maintain the same fonts, colors, and design elements across devices.
- Provide a uniform experience whether viewed on phone, tablet, or PC.

4. User Engagement
- Enable interactive features suited to each device, such as swipe gestures on mobile.
- Make navigation intuitive to improve user satisfaction and trust.
```

### Applications of Responsive Web Design
```css
1. E-commerce Websites: Provides smooth shopping experience across devices.
2. Educational Platforms: Enables learning access anytime on any device.
3. Business Websites: Maintains consistent brand presence and accessibility.
4. Blogs & News Websites: Ensures better readability and content presentation.
5. Web Applications: Allows dashboards and tools to work on all screen sizes.
6. Portfolio Websites: Showcases work effectively across devices.
```

### Techniques for Building Responsive Web Design
Responsive web design focuses on adapting layouts and content to ensure a seamless user experience across all screen sizes and devices.

`1. Use Fluid Grids`
```css
1. Use fluid grid systems instead of fixed-width layouts so the design adapts to different screen sizes.
2. Apply percentage-based widths to ensure elements resize proportionally across devices.

Example:
/* Write CSS Here */
.container {
  width: 90%;
  margin: auto;
}
```

`2. Use Flexible Images`
```css
1. Ensure images and media scale properly within their containers.
2. Use CSS properties like max-width: 100% to prevent content from overflowing the layout.

Example:
/* Write CSS Here */
img {
  max-width: 100%;
  height: auto;
}
```

`3. Apply Media Queries`
```css
1. Use CSS media queries to target different screen sizes and device orientations.
2. Modify layouts, fonts, and colors based on screen width, height, or resolution.
3. Improve usability by applying styles such as larger text on smaller screens.

Example:
@media (max-width: 768px) {
  body {
    font-size: 14px;
  }
}
```

`4. Prioritize Touchscreens`
```css
1. Make buttons and interactive elements large enough for comfortable touch interaction.
2. Place navigation elements in easily accessible areas to improve mobile usability.

Example:
button {
  padding: 12px 20px;
  font-size: 16px;
}
```

`5. Test Responsiveness`
```css
1. Test the website on multiple devices and browsers for consistent behavior.
2. Use tools and emulators to preview performance across different screen sizes.
3. Make necessary adjustments based on testing results to improve usability.
```

<b>Example:</b>
```css
<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Arial;
}

.container {
  display: flex;
}

.box {
  width: 33.33%;
  padding: 20px;
  background-color: lightgray;
  border: 1px solid black;
}

/* Responsive */
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }

  .box {
    width: 100%;
  }
}
</style>
</head>
<body>

<h2>Responsive Design Example</h2>

<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>

</body>
</html>
```

## 5. CSS Positioning Elements
CSS positioning is used to control the placement of elements on a web page. It allows elements to be positioned relative to the normal document flow, the browser window, or other elements.

### Features:
```css
1. The position property defines how an element is positioned.
2. Common position values include static, relative, absolute, fixed, and sticky.
3. Positioning works with properties like top, right, bottom, and left.
4. It helps create flexible layouts, overlays, and responsive designs.
```

### Types of Positioning
`1. Static Positioning :` Static is the default position of an element. It does not accept properties like top, left, right, or bottom.
```css
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

Explanation:
- The boxes follow the normal flow of the document.
- There’s no overlap or displacement of elements.1
```

`2. Relative Positioning :` Relative positioning places an element relative to its normal position. You can move it using top, left, right, or bottom.
```css
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

- Box 2 is shifted 20px down and 30px to the right from its normal position.
```

`3. Absolute Positioning :` Absolute positioning removes the element from the document flow and places it relative to the nearest ancestor with a positioning context (relative, absolute, or fixed).
```css
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

Explanation:
- The pink box (.absolute) is positioned 50px down and 50px right within the .container.
- It does not affect other elements in the flow.
```

`4. Fixed Positioning :` Fixed positioning removes the element from the flow and positions it relative to the viewport. It remains in place even when the page scrolls.
```css
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

- The fixed element stays at the top-right corner of the viewport even as the user scrolls.
```

`5. Sticky Positioning :` Sticky positioning switches between relative and fixed based on the scroll position.
```css
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

- The sticky element stays at the top of the viewport as you scroll but only within its containing element.
```

## 6. CSS Specificity
CSS specificity is the set of rules browsers use to determine which CSS style is applied when multiple rules target the same element. The rule with the higher specificity value takes priority.

### Features:
```css
1. Inline styles have the highest specificity.
2. ID selectors override class, attribute, and element selectors.
3. Class selectors override element and pseudo-element selectors.
4. When specificity is equal, the rule written last is applied.
```

### CSS Specificity Rules
`1. Inline CSS`
```css
1. Inline CSS applied directly to an HTML element using the style attribute.
2. Has the highest specificity and overrides both internal and external CSS rules.
```

`2. Internal CSS`
```css
1. Internal stylesheets defines inside the <style> tag within an HTML document.
2. Specificity depends on the selector used (ID > class > element).
3. Overrides external CSS when selectors have the same specificity.
```

`3. External CSS`
```css
1. External CSS Written in a separate .css file and linked using the <link> tag.
2. Used to style multiple pages consistently.
3. Specificity depends on the selectors used and is lower than inline and internal CSS.
```
<b>Rule:</b>
```css
1. The Specificity is mainly determined by the Selectors themselves, rather than whether the styles are defined internally within a <style> tag or externally in a separate CSS file, in the case of specificity for external or internal CSS rules. 

2. If the selectors used in External and Internal CSS contain the same components, then their specificity will be the same, and it will not be affected by the location of the CSS rule.

3. If any conflict exists for the styles of the same element, then the styles will be implemented based on the order of inclusion in the HTML document.

4. When two or more selectors have equal specificity, then the last(latest) one counts.

5. Universal selectors (like body and inherited selectors) have the least specificity.
```

### Specificity Hierarchy
| **Priority Level** | **Type**                            | **Description**                                                                                   |
| ------------------ | ----------------------------------- | ------------------------------------------------------------------------------------------------- |
| Highest            | Inline Style                        | Directly applied using the `style` attribute inside HTML elements                                 |
| High               | ID Selectors                        | Targets elements using a unique `id` attribute                                                    |
| Medium             | Classes, Pseudo-classes, Attributes | Targets using class names (`.class`), pseudo-classes (`:hover`), and attributes (`[type="text"]`) |
| Low                | Elements and Pseudo-elements        | Applies to HTML elements (`div`, `p`) and pseudo-elements (`::before`, `::after`)                 |

<b>Example:</b>
```css
<!DOCTYPE html>
<html>

<head>
    <style type="text/css">
        h1 {
            background-color: red;
            color: white;
        }

        #second {
            background-color: black;
            color: white;
        }

        .third {
            background-color: pink;
            color: blue;
        }

        #second1 {
            color: blue;
        }

        .third1 {
            color: red;
        }
    </style>
</head>

<body>
    <h1 id="second" class="third">
        ID has highest priority.
    </h1>
    <h1>
        Element selectors has lowest priority.
    </h1>
    <h1 class="third">
        Classes have higher priority
        than element selectors.
    </h1>

    <h2 style="color: green;" 
        id="second1"
        class="third1">
        Inline CSS has highest priority.
      </h2>
</body>

</html>
```

## 7. CSS Variables
CSS variables (custom properties) are reusable values defined with two dashes (--) that make your CSS code efficient and easier to maintain.

### Features:
```css
1. Store values like colors, sizes, or fonts in one place for centralized updates.
2. Use var() to apply these variables anywhere in your CSS.
3. Improve code readability and consistency across your styles.

Syntax:
var( --custom-name, value );

Parameters:
1. --custom-name: (Required) The name of the custom property, starting with two dashes (--).
2. value: (Optional) A value used if the custom property is not defined or is invalid.
```

<b>Example:</b>
```css
<!DOCTYPE html>
<html>
<head>
<style>

/* Define variables */
:root {
  --primary-color: #3498db;
  --secondary-color: #2ecc71;
  --font-size: 18px;
}

/* Use variables */
body {
  background-color: var(--secondary-color);
  font-size: var(--font-size);
}

h1 {
  color: var(--primary-color);
}

button {
  background-color: var(--primary-color);
  color: white;
  padding: 10px;
  border: none;
}

</style>
</head>
<body>

<h1>CSS Variables Example</h1>
<button>Click Me</button>

</body>
</html>
```
### Best Practices for CSS Variables
```css
1. Define Variables in :root: Declare global variables within the :root selector to ensure they are accessible throughout your stylesheet.

2. Use Descriptive Naming: Choose clear and descriptive names for variables to enhance readability and maintainability.

3. Leverage the Cascade: Take advantage of CSS variables' ability to inherit and be overridden within specific scopes, allowing for flexible theming and component styling.
```

## 8. CSS Inheritance
Inheritance in CSS allows certain properties to pass from parent elements to their child elements automatically. This helps maintain consistency and reduces repetitive code.

### Features:
```css
1. Use inherited properties like color, font-family, and line-height on parent elements to style multiple child elements at once.
2. Apply inherit value explicitly (e.g., color: inherit;) to force inheritance where it's not default.
3. Structure HTML logically so parent elements control common styles, improving maintainability.
```

<b>Syntax: </b>
```css
<style>
    #parentclass {
        color: red;
    }
</style>
<div id="parentclass">
    Parent Div
    <div id="div1Child">Child Div 1</div>
    <div id="div2Child">Child Div 2</div>
</div>

Explanation:
- Parent has color: red.
- color is an inheritable CSS property.
- Child divs have no color set.
- They automatically inherit red from the parent.
- Result: child divs display red text.
```

<b>Example:</b>
```css
<html>
<head>
    <style>
        #parentclass {
            color: black;
        }
        #child1 {
            color: green;
        }
        #childchild1 {
            color: red;
        }
    </style>
</head>
<body>
    <div id="div1">
        Parent
        <div id="child1">
            Child 1
            <div id="childchild1">
                Child Child 1
                <div id="childchildchild1">
                    Child Child Child
                </div>
            </div>
            <div id="childchild2">
                Child Child 2
            </div>
        </div>
        <div id="child2">
            Child 2
        </div>
    </div>
</body>
</html>

Exaplanation:
- Parent has color: black.
- color is an inheritable CSS property.
- #child1 has color: green → overrides parent (specificity).
- #child2 has no color -inherits black from parent.
- #childchild1 has color: red -overrides both parent and child1.
- Result: child1 shows green, child2 shows black, childchild1 shows red.
```
<b>Limitations:</b>
```css
We cannot inherit all the properties /rules of CSS. All font-* properties are naturally inherited like

1. font-size
2. font-family
3. font-weight
4. font-style, etc.

5. The color property is also inherited.
- CSS properties such as height, border, padding, margin, width, etc. are not inherited naturally. We can do inheritance on noninheritable CSS properties. We use inherit for doing so.
```

## 9. CSS 3D Transforms
CSS 3D transforms are used to manipulate HTML elements in three dimensions by rotating them along the x-axis, y-axis, and z-axis. There are three main types of transformation which are listed below:

```csss
1. rotateX(): Rotates an element around its X-axis.
2. rotateY(): Causes rotation around the Y-axis.
3. rotateZ(): Enables rotation along the Z-axis.
```

### Methods
`The rotateX() Method :` The rotateX() method in CSS is used to rotate an HTML element around its X-axis, which is horizontal. 
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: orange;
            transform: rotateX(45deg);
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- rotateX(45deg): Rotates the element 45 degrees downward around the X-axis.
- This creates a 3D tilt effect, making the top edge move backward.
```

`2. The rotateY() Method :` The rotateY() method in CSS is used to rotate an HTML element around its vertical Y-axis. This method allows the element to flip side to side, creating a mirror-like rotation effect.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: green;
            transform: rotateY(45deg);
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- rotateY(45deg): Applies a 45-degree rotation around the Y-axis, causing the left side of the box to move towards the viewer and the right side to move away.
- This rotation provides a visual effect of the element spinning from left to right.
```

`3. The rotateZ() Method :` The rotateZ() method in CSS is used to rotate an HTML element around its Z-axis, which is perpendicular to the screen. This rotation affects the element as if it were spinning flat on the screen.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: red;
            transform: rotateZ(45deg);
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- rotateZ(45deg): Rotates the box 45 degrees around the Z-axis, creating a twist as if turning a dial.
- This rotation pivots the element around its center, altering its orientation on the plane of the screen.
```

## 10. CSS Transitions
CSS transitions are used to create smooth animations between two states of an element, enhancing interactivity and user experience.

### Features:
```css
1. Transitions can animate properties like color, size, and position.

2. Use selectors and pseudo-classes (e.g., :hover) to trigger transitions.

3. Key transition properties include transition-property, transition-duration, transition-timing-function, and transition-delay.

Example:
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            transition: background-color 0.5s;
        }
        .box:hover {
            background-color: green;
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

4. The .box class defines a square <div> with a blue background and a transition effect for the background-color property over 0.5 seconds.

5. When the user hovers over the <div>, the :hover pseudo-class changes the background color to green, triggering the transition.
```

### CSS Transition Properties
`1. transition-property :` This property allows you to select the CSS properties that you want to animate during the transition(change). 
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            transition-property: width;
            transition-duration: 0.5s;
        }
        .box:hover {
            width: 200px;
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- The .box class defines a square <div> with a blue background.
- The transition-property is set to width, and transition-duration is set to 0.5s, enabling a smooth transition effect when the width changes.
- When the user hovers over the <div>, the :hover pseudo-class increases the width from 100px to 200px, triggering the transition.
```

<b> Syntax: </b>
```css
transition-property: none | all | property | property1, property2, ..., propertyN;

Values:

1. none is used to specify that no property should be selected.
2. all is used to specify all the properties to be selected.
3. We can specify a single property or a set of comma-separated properties property1, property2, ..., propertyN.
```

`2. transition-duration :` This property allows you to determine how long it will take to complete the transition from one CSS property to the other. 
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            transition-duration: 0.5s;
        }
        .box:hover {
            background-color: green;
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- The .box class defines a square <div> with a blue background and a transition duration of 0.5 seconds.
- When the user hovers over the <div>, the :hover pseudo-class changes the background color to green, and the transition occurs over 0.5 seconds.
```
<b>Syntax: </b>
```css
transition-duration: time;

- Here, time can be in seconds(s) or milliseconds(ms), you should use 's' or 'ms' after the number (without quotes).
```

`3. transition-timing-function :` Controls the speed and timing of a transition.
<br>
Defines how the change progresses (e.g., fast start, slow end).
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            transition: background-color 0.5s;
            transition-timing-function: ease-in-out;
        }
        .box:hover {
            background-color: green;
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- The .box class defines a square <div> with a blue background and a transition effect for the background-color property over 0.5 seconds.
- The transition-timing-function is set to ease-in-out, causing the transition to start and end slowly, with a faster change in the middle.
```
<b>Syntax: </b>
```css
transition-timing-function: ease|ease-in|ease-out|ease-in-out|linear|
step-start|step-end;
```

`4. transition-delay :` This property allows you to determine the amount of time to wait before the transition actually starts to take place. 
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            transition: background-color 0.5s;
            transition-delay: 1s;
        }
        .box:hover {
            background-color: green;
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Exaplanation:
- The .box class defines a square <div> with a blue background and a transition effect for the background-color property over 0.5 seconds.
- The transition-delay is set to 1s, causing a 1-second pause before the transition starts.
```
<b>Syntax: </b>
```css
transition-delay: time;
```

`Shorthand Property :` You can combine all four transition properties into a single shorthand property, which simplifies the code and ensures readability.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            transition: width 0.5s ease-in-out 1s;
        }
        .box:hover {
            width: 200px;
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- The transition shorthand combines width, duration (0.5s), ease-in-out, and delay (1s) into one property.
- On hover, the width smoothly changes from 100px to 200px after a 1-second delay.
- The ease-in-out makes the transition start and end slowly, with a faster middle phase.
```
<b>Syntax: </b>
```css
transition: (property name) | (duration) | (timing function) | (delay);

Explanation:
1. property: The CSS property you want to animate (e.g., width, background-color).
2. duration: The time the transition takes to complete (e.g., 0.5s for half a second).
3. timing-function: The speed curve of the transition (e.g., ease-in-out for a transition that starts and ends slowly).
4. delay: The time to wait before starting the transition (e.g., 1s for a one-second delay).
```

## 11. CSS Animations
CSS animations control the movement and appearance of elements on web pages. We can animate HTML elements without using JavaScript.

### Features:
```css
1. Use @keyframes to define the animation steps.
2. Apply animations with properties like animation-name and animation-duration.
3. Control the animation flow using animation-timing-function and animation-delay.
```
<b> Example:</b>
```css
<html>
<head>
	<style>
		.box {
			width: 100px;
			height: 100px;
			background-color: blue;
			animation: changeColor 3s infinite;
		}

		@keyframes changeColor {
			from {
				background-color: blue;
			}

			to {
				background-color: green;
			}
		}
	</style>
</head>

<body>
	<div class="box"></div>
</body>

</html>
```

### CSS Animation Properties
| **Property**                  | **Description**                                                                                                                  |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **@keyframes**                | The @keyframes rule in CSS is used to specify the animation rule.                                                                |
| **animation-name**            | It is used to specify the name of the @keyframes describing the animation.                                                       |
| **animation-duration**        | It is used to specify the time duration it takes animation to complete one cycle.                                                |
| **animation-timing-function** | It specifies how animations make transitions through keyframes. Values include linear, ease, ease-in, ease-out, and ease-in-out. |
| **animation-delay**           | It specifies the delay before the animation starts.                                                                              |
| **animation-iteration-count** | This specifies the number of times the animation will be repeated.                                                               |
| **animation-direction**       | It defines the direction of the animation (normal, reverse, alternate, alternate-reverse).                                       |
| **animation-fill-mode**       | It defines how styles are applied before and after animation (none, forwards, backwards, both).                                  |
| **animation-play-state**      | This property specifies whether the animation is running or paused.                                                              |

`1. @keyframes Rule :` The @keyframes rule defines how an element's styles change over time during an animation.
```css
<html>
<head>
	<style>
		.box {
			width: 100px;
			height: 100px;
			background-color: blue;
			animation: changeColor 3s infinite;
		}

		@keyframes changeColor {
			from {
				background-color: blue;
			}

			to {
				background-color: green;
			}
		}
	</style>
</head>

<body>
	<div class="box"></div>
</body>

</html>

Explanation:
- The .box class creates a blue square and applies the changeColor animation that lasts 3 seconds and repeats infinitely.
- The @keyframes changeColor rule changes the background color from blue to green.
```
<b>Syntax: </b>
```css
@keyframes animation-name {    from {        /* Initial Styles */    }    to {        /* Final Styles */    }}

- The from defines the starting styles, and to defines the ending styles.
- You can also use percentage values to specify intermediate steps.
```

`2. animation-name Property :` The animation-name property specifies the name of the @keyframes animation to apply to an element.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            animation-name: moveRight;
            animation-duration: 2s;
            animation-iteration-count: infinite;
        }

        @keyframes moveRight {
            from {
                transform: translateX(0);
            }
            to {
                transform: translateX(200px);
            }
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
The .box class applies the moveRight animation to the <div>.
The animation-name links the element to the @keyframes moveRight sequence.
The box moves horizontally from its original position to 200px to the right over 2 seconds, repeating infinitely.
```
<b>Syntax: </b>
```css
animation-name: animationName;
```

`3. animation-timing-function property :` The animation-timing-function property controls the speed curve of an animation, defining how the animation progresses over its duration.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            animation-name: slide;
            animation-duration: 3s;
            animation-timing-function: ease-in;
            animation-iteration-count: infinite;
        }

        @keyframes slide {
            from {
                transform: translateX(0);
            }
            to {
                transform: translateX(300px);
            }
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- The .box class applies the slide animation to the <div>.
- The animation-timing-function: ease-in; makes the animation start slowly and then speed up.
```
<b>Syntax: </b>
```css
animation-timing-function: timingFunction;
```

`4. animation-delay property :` The animation-delay property specifies a delay before an animation starts, controlling when the animation begins after being triggered.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            animation-name: fadeIn;
            animation-duration: 2s;
            animation-delay: 1s;
            animation-iteration-count: infinite;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:

- The .box element is set to fade in using the fadeIn animation.
- The animation-delay: 1s; delays the start of the animation by one second.
- The animation lasts for 2 seconds and repeats infinitely.
```
<b>Syntax: </b>
```css
animation-delay: time;
```

`5. animation-iteration-count property :` The animation-iteration-count property specifies how many times an animation should repeat.
```css
<html>
<head>
	<style>
		.box {
			width: 100px;
			height: 100px;
			background-color: blue;
			animation: bounce 2s infinite;
		}
		@keyframes bounce {
			0% {
				transform: translateY(0);
			}

			50% {
				transform: translateY(-50px);
			}

			100% {
				transform: translateY(0);
			}
		}
	</style>
</head>
<body>
	<div class="box"></div>
</body>

</html>

Explanation:
- The .box element uses the bounce animation that lasts 2 seconds.
- animation-iteration-count: infinite; makes the animation loop endlessly.
```
<b>Syntax: </b>
```css
animation-iteration-count: number | infinite;
```

`6. animation-direction property :` The animation-direction property specifies whether an animation should play forward, backward, or alternate between the two directions.
```css
<html>
<head>
	<style>
		.box {
			width: 100px;
			height: 100px;
			background-color: blue;
			animation: move 2s infinite;
			animation-direction: alternate;
		}
		@keyframes move {
			from {
				transform: translateX(0);
			}

			to {
				transform: translateX(200px);
			}
		}
	</style>
</head>
<body>
	<div class="box"></div>
</body>
</html>

Explanation:
- The .box element moves from its original position to 200px to the right.
- animation-direction: alternate; makes the animation play forward on the first iteration and then backward on the next, creating a back-and-forth motion.
```
<b>Syntax: </b>
```css
animation-direction: normal | reverse | alternate | alternate-reverse;
```

`7. animation-fill-mode property :` The animation-fill-mode property specifies how a CSS animation should apply styles to its target before and after it is executing.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            animation: move 3s forwards;
        }
        @keyframes move {
            from {
                transform: translateX(0);
            }
            to {
                transform: translateX(200px);
            }
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- The .box element moves from its original position to 200px to the right over 3 seconds.
- animation-fill-mode: forwards; ensures that the box retains the final state of the animation after it completes.
```
<b>Syntax: </b>
```css
animation-fill-mode: none | forwards | backwards | both;
```

`8. animation-play-state property :` The animation-play-state property controls whether an animation is running or paused.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            animation: spin 4s linear infinite;
            animation-play-state: paused;
        }

        .box:hover {
            animation-play-state: running;
        }

        @keyframes spin {
            from {
                transform: rotate(0deg);
            }
            to {
                transform: rotate(360deg);
            }
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- The .box element has a spin animation that rotates it 360 degrees over 4 seconds infinitely.
- animation-play-state: paused; initially pauses the animation.
```
<b>Syntax: </b>
```css
animation-play-state: running | paused;
```

`9. Animation Shorthand Property :` The animation shorthand property allows you to set all animation-related properties in a single declaration, making your CSS code cleaner and more concise.
```css
<html>
<head>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            animation: move 2s ease-in 1s infinite alternate forwards;
        }
        @keyframes move {
            from {
                transform: translateX(0);
                background-color: blue;
            }
            to {
                transform: translateX(200px);
                background-color: green;
            }
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Explanation:
- The .box class uses the animation shorthand to apply the move animation.
- The animation lasts for 2 seconds, starts after a 1-second delay, runs infinitely, alternates direction, and retains the final state.
- The box moves from its original position to 200px to the right and changes color from blue to green smoothly.
```
<b>Syntax: </b>
```css
animation: [animation-name] [animation-duration] [animation-timing-function] 
[animation-delay] [animation-iteration-count] [animation-direction] [animation-fill-mode]
[animation-play-state];
```

### Best Practices for CSS Animations
```css
1. Use Animations Purposefully: Apply animations to enhance user experience without causing distractions.
2. Animate Performance-Friendly Properties: Prefer animating properties like transform and opacity for smoother performance.
3. Ensure Accessibility: Provide options for users to reduce or disable animations to accommodate those with motion sensitivities.
```

## 12. CSS Functions
CSS functions are used to dynamically define or manipulate property values in stylesheets, making designs more flexible and responsive.
```css
1. Retrieve values like attributes with attr() or calculate sizes with calc().
2. Adjust colors using functions like rgb() or hsl().

Example:
<html>
<head>
    <style>
        .box {
            width: calc(50% - 10px);
            background: linear-gradient(to right, lightblue, lightgreen);
            height: 100px;
            border: 1px solid black;
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>

4. The calc() function dynamically calculates the width of the box as 50% of the parent element minus 10px.
5. The linear-gradient() function creates a smooth gradient background transitioning from light blue to light green.
```

### Function List:
| **Function**                  | **Description**                                            |
| ----------------------------- | ---------------------------------------------------------- |
| `attr()`                      | Returns the value of an attribute of the selected element. |
| `blur()`                      | Applies a blur effect to an element (usually images).      |
| `brightness()`                | Adjusts the brightness of an element.                      |
| `calc()`                      | Performs calculations to determine CSS values.             |
| `circle()`                    | Defines a circular shape (used in clip-path).              |
| `conic-gradient()`            | Creates a conic gradient background.                       |
| `contrast()`                  | Adjusts the contrast of an element.                        |
| `cubic-bezier()`              | Defines a custom animation timing curve.                   |
| `drop-shadow()`               | Adds a shadow effect to elements.                          |
| `ellipse()`                   | Defines an elliptical shape (used in clip-path).           |
| `env()`                       | Inserts environment variables (like safe-area).            |
| `grayscale()`                 | Converts an element to grayscale.                          |
| `hsl()`                       | Defines colors using Hue, Saturation, Lightness.           |
| `hsla()`                      | Defines colors with transparency (alpha).                  |
| `hue-rotate()`                | Rotates the color hue of an element.                       |
| `inset()`                     | Defines inset clipping (used with clip-path).              |
| `invert()`                    | Inverts colors of an element.                              |
| `linear-gradient()`           | Creates a linear gradient background.                      |
| `matrix()`                    | Applies 2D transformation matrix.                          |
| `matrix3d()`                  | Applies 3D transformation matrix.                          |
| `max()`                       | Returns the largest value.                                 |
| `min()`                       | Returns the smallest value.                                |
| `opacity()`                   | Sets transparency level.                                   |
| `perspective()`               | Adds perspective to 3D elements.                           |
| `polygon()`                   | Creates custom shapes using points.                        |
| `radial-gradient()`           | Creates a radial gradient background.                      |
| `repeating-conic-gradient()`  | Repeats conic gradients.                                   |
| `repeating-linear-gradient()` | Repeats linear gradients.                                  |
| `repeating-radial-gradient()` | Repeats radial gradients.                                  |
| `rgb()`                       | Defines colors using Red, Green, Blue.                     |
| `rgba()`                      | Defines colors with transparency.                          |
| `rotate()`                    | Rotates an element.                                        |
| `rotate3d()`                  | Rotates element in 3D space.                               |
| `rotateX()`                   | Rotates element along X-axis.                              |
| `rotateY()`                   | Rotates element along Y-axis.                              |
| `rotateZ()`                   | Rotates element along Z-axis.                              |
| `saturate()`                  | Adjusts color saturation.                                  |
| `scale()`                     | Resizes element in 2D.                                     |
| `scale3d()`                   | Resizes element in 3D.                                     |
| `scaleX()`                    | Scales along X-axis.                                       |
| `scaleY()`                    | Scales along Y-axis.                                       |
| `scaleZ()`                    | Scales along Z-axis.                                       |
| `sepia()`                     | Applies sepia effect.                                      |
| `skew()`                      | Skews element in 2D.                                       |
| `skewX()`                     | Skews horizontally.                                        |
| `skewY()`                     | Skews vertically.                                          |
| `translate()`                 | Moves element in X and Y directions.                       |
| `translate3d()`               | Moves element in 3D space.                                 |
| `translateX()`                | Moves element horizontally.                                |
| `translateY()`                | Moves element vertically.                                  |
| `translateZ()`                | Moves element in depth (Z-axis).                           |
| `url()`                       | Loads external resources (image, font, etc.).              |
| `var()`                       | Uses custom CSS variables.                                 |


### Best Practices for Using CSS Functions
```css
1. Use Functions Appropriately: Apply CSS functions like calc(), var(), and rgb() to enhance flexibility and maintainability in your stylesheets.
2. Maintain Readability: While functions add power, ensure your code remains readable by avoiding overly complex expressions.
3. Test Across Browsers: Some CSS functions may have varying levels of support; always test your styles across different browsers to ensure compatibility.
```

<b>Example:</b>
```css
<!DOCTYPE html>
<html>
<head>
<style>
.box {
  width: 200px;
  height: 200px;
  background: linear-gradient(to right, red, yellow);
  transform: rotate(20deg) scale(1.2);
  filter: blur(2px) brightness(120%);
  margin: 50px;
}
</style>
</head>
<body>

<div class="box"></div>

</body>
</html>

Explanation
- linear-gradient() → creates gradient background
- rotate() → rotates the box
- scale() → increases size
- blur() → adds blur effect
- brightness() → increases brightness
```