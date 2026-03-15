# Full stack | HTML

## HTML - 1#

Date - 31/01/2024

<aside>
💡 HTML - Hyper Text Markup Language,

</aside>

HTML provides structure to the content that appears on a website, such as images, text, or videos. Right-click on any page on the internet and choose “Inspect” and you will see HTML in a panel on your screen. As you continue learning, you can layer HTML with CSS and JavaScript to create visually compelling and dynamic websites.

### Vocab

HTML - Hyper Text Markup Language.

Markup language - A language that defines the structure of content.

HTML - The computer can interpret raw text that is wrapped in HTML elements.

HyperText - Text displayed on a computer or device that provides access to other documents via hyperlinks.

### Notes

- HTML is the first step in creating websites.
- Don't worry if it looks ugly at first.

---

## HTML Anatomy - 2#

Date - 31/04/2024

HTML is composed of elements these are what structure the webpage and define its content. 

![chrome_Zszm2h7aDK.png](chrome_Zszm2h7aDK.png)

### Vocab

Element - The Content between a tag is called an element

The Body - is the body for the page 

### Notes

- Elements have open and closing tag
- Elements have content

---

## HTML Structure - 3#

Date - 31/01/2024

The HTML structure is organized as a collection of family tree relationships. When an element is contained inside another element, it is considered a child of that element. The child element is nested inside the parent element. Understanding HTML hierarchy is important because child elements can inherit behavior and styling from their parent elements. You’ll learn more about webpage hierarchy when you start digging into CSS.

An example of a nested paragraph

```html
<!-- An example of a nested paragraph -->
<body>
  <p>This paragraph is a child of the body</p>
</body>
```

An example of more complicated nesting

```html
<!-- An example of more complicated nesting -->
<body>
  <div>
    <h1>Sibling to p, but also grandchild of body</h1>
    <p>Sibling to h1, but also grandchild of body</p>
  </div>
</body>
```

Headings in HTML are used for main headings and subheadings. In HTML, there are six different *headings*, or *heading elements*. They are used for a variety of purposes, from largest to smallest and for different types of content.

```html
<h1> — used for main headings. All other smaller headings are used for subheadings.
<h2>
<h3>
<h4>
<h5>
<h6>
```

### Vocab

child - Element inside a parent element.

hierarchy - Relationships between elements and their ancestors and descendants.

headings - In HTML, headings are used for main headings and subheadings.

div - Short for “division,” meaning a division of space or sections.

### Notes

- `div` elements are useful for grouping elements in HTML together.
- `div` elements don’t have a lot of visual representation, but are useful when you want to apply custom styles to HTML elements.
- With `div` elements you can group elements that share the same styles.

---

## Attributes - 4#

Date - 03/02/2024

Attributes allow us to expand an element’s tag and can be used in several ways, such as changing the styling or providing information.

An example of an attribute in use 

```html
<div id="intro">
  <h1>Introduction</h1>
</div>
```

### Vocab

Attribute - A way to expand an element’s tag.

id attribute - This attribute can be used to specify different content such as a `div` id and has several different purposes in HTML.

### Notes

- Attributes are content added to the opening tag of an element.

---

## Displaying text - 5#

Date - 03/02/2024

To display text in HTML we would normally use a paragraph tag.

This is an example of how text is displayed using a `p` tag and `span` element:

```html
<div>
  <h1>Technology</h1>
</div>
<div>
  <p><span>Self-driving cars</span> are anticipated to replace up to 2 million jobs over the next two decades.</p>
</div>
```

It’s best to use a `<span>` element when you want to target a specific piece of content that is *inline*, or on the same line as other text. 

## Styling Text

In HTML you can also style text using the `<em>` tag, which emphasizes text, while the `<strong>` tag highlights important text.

- The `<em>` tag will generally render as *italic* emphasis.
- The `<strong>` will generally render as **bold** emphasis.

This is an example of text being styled.

```html
<p><strong>The Nile River</strong> is the <em>longest</em> river in the world, measuring over 6,850 kilometers long (approximately 4,260 miles).</p>
```

## Line Breaks

Spacing between code in HTML does not affect the positioning of elements in the browser. If you need to change the spacing in the browser, use the HTML `<br>` tag.

## Unordered Lists

Unordered lists are a way you can display content in an organized, easy-to-read way using a `<ul>` element. A `ul` element should not hold raw text.

This is an example of a `ul`:

```html
<ul>
  <li>Limes</li>
  <li>Tortillas</li>
  <li>Chicken</li>
</ul>
```

Inside of a `ul` tag you put individual list items using the `li` tag.

## Ordered Lists

Ordered lists are similar to unordered lists, but instead of being bullet-pointed they are numbered. They are useful when you need to list different steps in a process or rank items from first to last.

This is an example of an ordered list

```html
<ol>
  <li>Preheat the oven to 350 degrees.</li>
  <li>Mix whole wheat flour, baking soda, and salt.</li>
  <li>Cream the butter, sugar in separate bowl.</li>
  <li>Add eggs and vanilla extract to bowl.</li>
</ol>
```

## Images

The `img` tag allows you to add an image to a website. Most elements use both opening and closing tags, but the image element is a self-closing tag, meaning it uses `/` at the end of the tag.

The image tag uses the `src` attribute.

```html
<img src="image-location.jpg" />
```

## Image Alts

When developing websites it’s a good idea to make your site accessible to all kinds of different users. You also need to keep in mind what happens when tech like screen readers encounters image tags.

An example of using image alts:

```html
<img src="#" alt="A field of yellow sunflowers" />
```

### Vocab

Paragraph - Contains a block of plain text.

span - Contains short pieces of text or other inline HTML.

Line breaks - Forces content onto a new line; does not affect the position of elements.

ul - An organized way to display list items.

Alt - Alternative attribute that describes an image.

### Notes

- A `ul` should not hold raw text.
- The `src` in the image is the *uniform resource locator* (URL) of the image.
- The `alt` attribute is for alternative text that describes the image.
- If an image fails to load on a page, the `alt` attribute will display a short description of the image.
- For visually impaired users, a screen reader will read the image’s description out loud.
- The `alt` attribute is also good for SEO because search engines cannot see images on sites as they crawl the internet.

---

## Videos - #

Date - 03/02/2024

Similar to the image element, HTML also allows videos to be displayed. Like the `<img>` element, videos use the `<video>` element, which also uses a `src` attribute with a link to the source.

This is an example of a video element in use

```html
<!-- The “Video not supported” text appears if a browser does not support video -->
<video src="myVideo.mp4" width="320" height="240" controls>
  Video not supported
</video>
```

### Vocab

WORD - definition

WORD - definition

### Notes

- Important notes
- 

### **Review**

Congratulations on completing the first lesson of HTML! You are well on your way to becoming a skilled web developer.

Let’s review what you’ve learned so far:

- **HTML** stands for **H**yper**T**ext **M**arkup **L**anguage and is used to create the structure and content of a webpage.
- Most HTML elements contain opening and closing tags with raw text or other HTML tags between them.
- HTML elements can be nested inside other elements. The enclosed element is the child of the enclosing parent element.
- Any visible content should be placed within the opening and closing `<body>` tags.
- Headings and sub-headings, `<h1>` to `<h6>` tags, are used to provide titles for sections of content.
- `<p>`, `<span>` and `<div>` tags specify text or blocks.
- The `<em>` and `<strong>` tags are used to emphasize text.
- Line breaks are created with the `<br>` tag.
- Ordered lists (`<ol>`) are numbered and unordered lists (`<ul>`) are bulleted.
- Images (`<img>`) and videos (`<video>`) can be added by linking to an existing source.

---

# Full-Stack | CSS

<aside>
💡 The goal of this unit is to introduce you to CSS, one of the languages essential to developing websites. You will learn how to apply styles to HTML documents using CSS.

</aside>

Date - 09/02/2024

Cascading Style Sheets or *CSS* is a language web developers use to style the HTML content on a web page.

```css
/* ThiS is an example of linking css pages to the main page in head element */
<link href="style.css" rel="stylesheet">
```

### Vocab

**CSS Anatomy** - The anatomy of [CSS](https://www.codecademy.com/resources/docs/css) style syntax applies to the two methods of incorporating CSS into a web-page:

RuleSet - A ruleset is defined within either the [HTML](https://www.codecademy.com/resources/docs/html) document itself, or in one or more separate files (known as stylesheets) that use the **.css** extension.

*Selector*—The beginning of the ruleset used to target the element that will be styled.

*Declaration Block*—The code in-between (and including) the curly braces (`{ }`) that contains the CSS declaration(s

*Declaration*—The group name for a property and value pair that applies a style to the selected element

*Property*—The first part of the declaration that signifies what visual characteristic of the element is to be modified.

*Value*—The second part of the declaration that signifies the value of the property

Inline styles - An inline style is set in a `style` [attribute](https://www.codecademy.com/resources/docs/html/attributes) and applies to individual [HTML elements](https://www.codecademy.com/resources/docs/html/elements) directly.

*Opening Tag*—The start of an [HTML element](https://www.codecademy.com/resources/docs/html/elements?page_req=catalog). This is the element that will be styled.

*Attribute*—The style [attribute](https://www.codecademy.com/resources/docs/html/attributes?page_req=catalog) is used to add CSS inline styles to an HTML element.

*Declaration*—The group name for a property and value pair that applies a style to the selected element.

*Property*—The first part of the declaration that signifies what visual characteristic of the element is to be modified.

*Value*—The second part of the declaration that signifies the value of the property.

### Notes

- This is an example of  CSS Ruleset - `p { color:blue; }`
- This is ane example of CSS `<p style="color: blue”`
- Its important to know inline styles are a quick way of styling an element but they are rarely used when making websites.
- 

## Internal stylesheet

css allows you to code in its own dedicated section with a style element nested inside of the head element this is known as internal styles.

```css
<head>
  <style>
		p {
      color: red;
      font-size: 20px;
    }
  </style>
</head>
```

## **External Stylesheet**

External style sheets are whats used to link the main index file to an external stylesheet called style.css

```css
/* Linking the CSS File */
<link href='style.css' rel='stylesheet'>
/* Rel means related to that page type */
```

## **Universal selector**

the *universal selector* selects all elements of *any* type.

The universal selector uses the `*` character in the same place where you specified the type selector in a ruleset, like so:

```css
* { 
	margin: 0px;
	padding: 0px;
}
```

## Class

CSS is not limited to selecting elements by their type. As you know, HTML elements can also have [attributes](https://www.codecademy.com/courses/learn-html/lessons/intro-to-html/exercises/attr-html). When working with HTML and CSS a [*class*](https://www.codecademy.com/resources/docs/html/classes?page_req=catalog) attribute is one of the most common ways to select an element.

```css
<p class='brand'>Sole Shoe Company</p>
```

## **Multiple Classes**

You can use multiple classes in the same css file, Luckily, it’s possible to add more than one class name to an HTML element’s `class` attribute.

```css
/* this is an example of multiple classes being used in an element */
<h1 class='title uppercase'>Top Vacation Spots</h1>
```

## ID

Oftentimes it’s important to select a single element with CSS to give it its own unique style. If an HTML element needs to be styled uniquely, we can give it an ID using the `id` attribute.``

```css
/* this is how you would use an id to style an element*/
<h1 id='large-title'> ... </h1>
/* this is selecting the id to style it */
#large-title {

}
```

## Attribute

Attributes are used on elements to add extra data or functionality such as `href` or `src` `class` and  `id` 

Attributes can be selected similarly to types, classes, and IDs.``

```css
/* an example of targeting an a tag in css */
[href]{
   color: magenta;
}
/* this is an example of elements with a src attribute with a value equaling a link to an image file */
img[src*='winter'] {
  height: 50px;
}

img[src*='summer'] {
  height: 100px;
}
```

## **Pseudo-class**

These are all examples of pseudo-class selectors in action! In fact, `:focus`, `:visited`, `:disabled`, and `:active` are all pseudo-classes. 

- user interaction,
- site navigation,
- and position,

All elements give a different state with pseudo-class

A pseudo-class can be attached to any selector. It is always written as a colon `:` followed by a name. For example `p:hover`.``

```css
/* this is an example of a pseudo-class in css being used */
a:hover { 
}
```

## Specificity

Specificity is the order by which the browser decides which CSS styles will be displayed.

A best practice in CSS is to style elements while using the lowest degree of specificity so that if an element needs a new style, it is easy to override.

IDs are the most specific selector in CSS, followed by classes, and finally, type. For example, consider the following HTML and CSS:``

```css
<h1 class='headline'>Breaking News</h1>

h1 {
  color: red;
}

.headline {
  color: firebrick;
}
/* the bottom 3 are utilizing each selector */
h5 {
  color: yellow;
}

.author-class {
  color: pink;
}

#author-id {
  color: cornflowerblue;
}
```

## Chaining

When writing CSS rules, it’s possible to require an HTML element to have two or more CSS selectors at the same time. This is done by combining multiple selectors, which we will refer to as chaining. For instance, if there was a `special` class for `<h1>` elements, the CSS would look like below:``

```css
h1.special {

}
```

## **Descendant Combinator**

In addition to chaining selectors to select elements, CSS also supports selecting elements that are nested within other HTML elements, also known as *descendants*. For instance, consider the following HTML``

```css

<ul class='main-list'>
  <li> ... </li>
  <li> ... </li>
  <li> ... </li>
</ul>
/* The nested <li> elements are descendants of the <ul> element and can be selected with the descendant combinator like so: */
.main-list li {

}
```

## **Chaining and Specificity**

instead of selecting all `<h5>` elements, you selected only the `<h5>` elements nested inside the `.description` elements. This CSS selector was more specific than writing only `h5`. Adding more than one tag, class, or ID to a CSS selector increases the specificity of the CSS selector.

For instance, consider the following CSS:

```css
p {
  color: blue;
}

.main p {
  color: red;
}

parent-selector descendant-selector {
  declaration
}
```

**Multiple Selectors**

this is an example of using multiple selectors 

```css
h1, 
.menu {
  font-family: Georgia;
}
or 
h1, li { 
}
```

---

## **Introduction To Visual Rules** - 1#

Date - 15/02/2024

Visual Rules is a way of understand how css works better to design websites

### Vocab

**Font Family** - the style of font you use

**Font Size** - this modifies the font size to set the text to the size you choose 

**Font Weigt -** this controls how bold or thin the text will appear 

**Text Align -** No matter how much styling is used text always appears on the left side of the container in which it resides. 

**Opacity -** This is the measure of how transparent an element is

**Background Image -** css allows you to change the background image of an element

**Important -** `!important` can be applied to specific declarations, instead of full rules. It will override *any* style no matter how specific it is.

### Notes

- he `text-align` property will align text to the element that holds it, otherwise known as its *parent*.
- Opacity : from 0 to 1, with 1 representing 100%, or fully visible and opaque, and 0 representing 0%, or fully invisible.
- The `background-image` property will set the element’s background to display an image.

## **Color and Background Color**

Before discussing the specifics of color, it’s important to make two distinctions about color. Color can affect the following design aspects: 

- Foreground color : Foreground color is the color that an element appears in. For example, when a heading is styled to appear green, the *foreground color* of the heading has been styled.
- Background color: Conversely, when a heading is styled so that its background appears yellow, the *background color* of the heading has been styled.

## Background Image

```css
.main-banner {
  background-image: url('https://www.example.com/image.jpg');
}
```

## Important

An example of the Important property being used

```css
p {
  color: blue !important;
}
```

### **Review Visual Rules**

- The [`font-family`](https://www.codecademy.com/resources/docs/css/typography/font-family) property defines the typeface of an element.
- [`font-size`](https://www.codecademy.com/resources/docs/css/typography/font-size) controls the size of text displayed.
- [`font-weight`](https://www.codecademy.com/resources/docs/css/typography/font-weight) defines how thin or thick text is displayed.
- The [`text-align`](https://www.codecademy.com/resources/docs/css/typography/text-align) property places text in the left, right, or center of its parent container.
- Text can have two different color attributes: [`color`](https://www.codecademy.com/resources/docs/css/colors/color) and [`background-color`](https://www.codecademy.com/resources/docs/css/background/background-color). `color` defines the color of the text, while `background-color` defines the color behind the text.
- CSS can make an element transparent with the [`opacity`](https://www.codecademy.com/resources/docs/css/colors/opacity) property.
- CSS can also set the background of an element to an image with the [`background-image`](https://www.codecademy.com/resources/docs/css/background/background-image) property.
- The `!important` flag will override any style, however it should almost never be used, as it is extremely difficult to override.

---

## **Introduction to the Box Model** - 2#

Date - 15/02/2024

Browsers load html elements with default position elements. But this can sometimes lead to bad user experience. The box model is a important concept to understand how elements are positioned and displayed on a website.

1. The dimensions of an element’s box.
2. The [borders](https://www.codecademy.com/resources/docs/css/borders) of an element’s box.
3. The paddings of an element’s box.
4. The [margins](https://www.codecademy.com/resources/docs/css/margins) of an element’s box.

![Screenshot 2024-02-15 at 10.11.49.png](Screenshot_2024-02-15_at_10.11.49.png)

### Vocab

WORD - definition

WORD - definition

### Notes

- Important notes
- 

## **The Box Model**

The model includes the content area’s size (*width* and *height*) 

1. `padding`: The amount of space between the content area and the border.
2. `border`: The thickness and style of the border surrounding the content area and padding.
3. `margin`: The amount of space between the border and the outside edge of the element.

## Borders

A [*border*](https://www.codecademy.com/resources/docs/css/borders/border) is a line that surrounds an element, like a frame around a painting. [Borders](https://www.codecademy.com/resources/docs/css/borders) can be set with a specific [`width`](https://www.codecademy.com/resources/docs/css/sizing/width), `style`, and

- `width`—The thickness of the border. A border’s thickness can be set in pixels or with one of the following keywords: `thin`, `medium`, or `thick`.
- `style`—The design of the border. Web browsers can render any of [10 different styles](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style#Values). Some of these styles include: `none`, `dotted`, and `solid`.
- `color`—The color of the border. Web browsers can render [colors](https://www.codecademy.com/resources/docs/css/colors) using a few different formats, including [140 built-in color keywords](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value).

## **Border Radius**

Ever since we revealed the borders of boxes, you may have noticed that the borders highlight the true shape of an element’s box: square. Thanks to CSS, a border doesn’t have to be square.

```css
div.container {
  border: 3px solid blue;
  border-radius: 5px;
}
```

## **Padding Shorthand**

A declaration that uses multiple properties as values is known as a *shorthand property*.

Padding shorthand lets you specify all of the `padding` properties as values on a single line:

- [`padding-top`](https://www.codecademy.com/resources/docs/css/padding/padding-top)
- [`padding-right`](https://www.codecademy.com/resources/docs/css/padding/padding-right)
- [`padding-bottom`](https://www.codecademy.com/resources/docs/css/padding/padding-bottom)
- [`padding-left`](https://www.codecademy.com/resources/docs/css/padding/padding-left)
    
    ```css
    /* an example of padding short hand */
    p.content-header {
      padding: 6px 11px 4px 9px;
    }
    /* this is an example of margin short hand similar to padding short hand */
    p {
      margin: 6px 10px 5px 12px;
    }
    ```
    

In the example above, the four values `6px 11px 4px 9px` correspond to the amount of padding on each side, in a clockwise rotation. In order, it specifies the padding-top value (`6px`), the padding-right value (`11px`), the padding-bottom value (`4px`), and the padding-left value (`9px`) of the content.

## Auto Margin

An example of auto margin being used

In the example above, `margin: 0 auto;` will center the divs in their containing elements. The 0 sets the top and bottom margins to 0 pixels. The `auto` value instructs the browser to adjust the left and right margins until the element is centered within its containing element.

```css
div.headline {
  width: 400px;
  margin: 0 auto;
}
```

## **Margin Collapse**

As you have seen, [padding](https://www.codecademy.com/resources/docs/css/padding/padding) is space added inside an element’s [border](https://www.codecademy.com/resources/docs/css/borders/border), while [margin](https://www.codecademy.com/resources/docs/css/margins/margin) is space added outside an element’s border. One additional difference is that top and bottom [margins](https://www.codecademy.com/resources/docs/css/margins), also called vertical margins, *collapse*, while top and bottom padding does not.

![Screenshot 2024-02-15 at 11.20.28.png](Screenshot_2024-02-15_at_11.20.28.png)

Horizontal margins (left and right), like padding, are always displayed and added together. For example, if two divs with ids `#div-one` and `#div-two`, are next to each other, they will be as far apart as the sum of their adjacent margins.

```css
#img-one {
  margin-right: 20px;
}

#img-two {
  margin-left: 20px;
}
```

## **Minimum and Maximum Height and Width**

Web pages can be viewed through displayed of different screen size 

- [`min-width`](https://www.codecademy.com/resources/docs/css/sizing/min-width)—this property ensures a minimum [width](https://www.codecademy.com/resources/docs/css/sizing/width) of an element’s box.
- [`max-width`](https://www.codecademy.com/resources/docs/css/sizing/max-width)—this property ensures a maximum width of an element’s box.

## **Resetting Defaults**

All major web browsers have a default stylesheet they use in the absence of an external stylesheet. These default stylesheets are known as *user agent stylesheets*. In this case, the term [*user agent*](https://en.wikipedia.org/wiki/User_agent) is a technical term for the browse

```css
* {
  margin: 0;
  padding: 0;
}
```

## **Visibility**

Elements can be hidden from view with the [`visibility`](https://www.codecademy.com/resources/docs/css/visibility) property.

The `visibility` property can be set to one of the following values:

- `hidden` — hides an element.
- `visible` — displays an element.
- `collapse` — collapses an element.

```css
<ul>
  <li>Explore</li>
  <li>Connect</li>
  <li class="future">Donate</li>
</ul>
/* example of hiding an element */
.future {
  visibility: hidden;
}
```

Review / Summary 

### **Review**

In this lesson, we covered the four properties of the box model: height and [width](https://www.codecademy.com/resources/docs/css/sizing/width), [padding](https://www.codecademy.com/resources/docs/css/padding/padding), [borders](https://www.codecademy.com/resources/docs/css/borders), and [margins](https://www.codecademy.com/resources/docs/css/margins). Understanding the [box model](https://www.codecademy.com/resources/docs/css/box-model) is an important step towards learning more advanced HTML and CSS topics. Let’s take a minute to review what you learned:

- The box model comprises a set of properties used to create space around and between HTML elements.
- The height and width of a content area can be set in pixels or percentages.
- Borders surround the content area and padding of an element. The color, style, and thickness of a [border](https://www.codecademy.com/resources/docs/css/borders/border) can be set with CSS properties.
- Padding is the space between the content area and the border. It can be set in pixels or percent.
- Margin is the amount of spacing outside of an element’s border.
- Horizontal margins add, so the total space between the borders of adjacent elements is equal to the sum of the right [margin](https://www.codecademy.com/resources/docs/css/margins/margin) of one element and the left margin of the adjacent element.
- Vertical margins collapse, so the space between vertically adjacent elements is equal to the larger margin.
- `margin: 0 auto` horizontally centers an element inside of its parent content area, if it has a width.
- The [`overflow`](https://www.codecademy.com/resources/docs/css/overflow/overflow) property can be set to [`display`](https://www.codecademy.com/resources/docs/css/display), `hidden`, or `scroll`, and dictates how HTML will render content that overflows its parent’s content area.
- The [`visibility`](https://www.codecademy.com/resources/docs/css/visibility) property can hide or show elements.

---

## **The Box Model in DevTools** - 3#

Date - 16/02/2024

All HTML elements are boxes made up of four components: a content container, padding, border, and margin. In our [Box Model lesson](https://www.codecademy.com/courses/learn-css/lessons/box-model-intro/exercises/box-model-intro) we introduce these four properties and use them to position elements on a website. If you have not taken this lesson, we recommend you do so now, before continuing.

**1. View Box Model Dimensions with DevTools**

![Untitled](Untitled.png)

### Vocab

WORD - definition

WORD - definition

### Notes

- Important notes
- 

**2. Modify Box Dimensions** 

![Untitled](Untitled%201.png)

## Position

he default position of an element can be changed by setting its `position` property. The `position` property can take one of five values:

- `static` - the default value (it does not need to be specified)
- `relative`
- `absolute`
- `fixed`
- `sticky`

## **Position: Relative**

This value allows you to position an element *relative* to its default static position on the web page.

```css
.green-box {
  background-color: green;
  position: relative;
}
```

## Position: Absolute

Another way of modifying the position of an element is by setting its position to `absolute`.

When an element’s position is set to `absolute`, all other elements on the page will ignore the element and act like it is not present on the page. The element will be positioned relative to its closest positioned parent element, while offset properties can be used to determine the final position from there. Take a look at the image below:

## Position: fixed

When an element’s position is set to `absolute`, as in the last exercise, the element will scroll with the rest of the document when a user scrolls.

We can *fix* an element to a specific position on the page (regardless of user scrolling) by setting its position to `fixed`, and accompanying it with the familiar offset properties [`top`](https://www.codecademy.com/resources/docs/css/position/top), [`bottom`](https://www.codecademy.com/resources/docs/css/position/bottom), [`left`](https://www.codecademy.com/resources/docs/css/position/left), and [`right`](https://www.codecademy.com/resources/docs/css/position/right).

```css
.title {
  position: fixed;
  top: 0px;
  left: 0px;
}
```

## Position: Sticky

The `sticky` value is another position value that keeps an element in the document flow as the user scrolls, but *sticks* to a specified position as the page is scrolled further. This is done by using the `sticky` value along with the familiar offset properties, as well as one new one.

```css
.box-bottom {
  background-color: darkgreen;
  position: sticky;
  top: 240px;
}
```

## Z index

The [`z-index`](https://www.codecademy.com/resources/docs/css/position/z-index) property controls how far back or how far forward an element should appear on the web page when elements overlap. This can be thought of as the *depth* of elements, with deeper elements appearing behind shallower elements.

The `z-index` property accepts integer values. Depending on their values, the integers instruct the browser on the order in which elements should be layered on the web page.

```css
.blue-box {
  background-color: blue;
  position: relative;
  z-index: 1;
}

.green-box {
  background-color: green;
  position: relative;
  top: -170px;
  left: 170px;
}
```

In the example above, we set the `.blue-box` position to `relative` and the z-index to 1. We changed position to `relative`, because the `z-index` property does *not* work on static elements. The z-index of `1` moves the `.blue-box` element forward, because the `z-index` value has not been explicitly specified for the `.green-box` element, which means it has a default `z-index` value of 0. Take a look at the example image below

![Untitled](Untitled%202.png)

## **Inline Display**

we’ll cover three values for the `display` property: `inline`, `block`, and `inline-block`

The default `display` for some elements, such as `<em>`, `<strong>`, and `<a>`, is called *inline*.

```css
To learn more about <em>inline</em> elements, read <a href="#">MDN documentation</a>.
```

CSS display property provides the ability to make any elements an inline element.

An example of display inline

```css
h1 { 
display: inline;
} 
```

## Display: Inline-block

The third value for the `display` property is `inline-block`. Inline-block display combines features of both inline and block elements. Inline-block elements can appear next to each other and we can specify their dimensions using the `width` and `height` properties. Images are the best example of default inline-block elements.

An example of inline block being used 

```css
<div class="rectangle">
  <p>I’m a rectangle!</p>
</div>
<div class="rectangle">
  <p>So am I!</p>
</div>
<div class="rectangle">
  <p>Me three!</p>
</div>

.rectangle {
  display: inline-block;
  width: 200px;
  height: 300px;
}
```

## Float

The `float` property is commonly used for wrapping text around an image. Note, however, that moving elements left or right for layout purposes is better suited for tools like CSS [grid](https://www.codecademy.com/resources/docs/css/grids/grid) and [flexbox](https://www.codecademy.com/resources/docs/css/flexbox), which you’ll learn about later on. 

The `float` property is often set using one of the values below:

- [`left`](https://www.codecademy.com/resources/docs/css/position/left) - moves, or [floats](https://www.codecademy.com/resources/docs/css/floats), elements as far left as possible.
- [`right`](https://www.codecademy.com/resources/docs/css/position/right) - moves elements as far right as possible.

![Untitled](Untitled%203.png)

```css
.green-section {
  width: 50%;
  height: 150px;
}

.orange-section {
  background-color: orange;
  width: 50%;
  float: right;
}
```

## Clear Property

The `float` property can also be used to float multiple elements at once. However, when multiple floated elements have different heights, it can affect their layout on the page. Specifically, elements can “bump” into each other and not allow other elements to properly move to the left or right.

The `clear` property specifies how elements should behave when they bump into each other on the page. It can take on one of the following values:

- `left`—the left side of the element will not touch any other element within the same containing element.
- `right`—the right side of the element will not touch any other element within the same containing element.
- `both`—neither side of the element will touch any other element within the same containing element.
- `none`—the element can touch either side.

```css
div {
  width: 200px;
  float: left;
}

div.special {
  clear: left;
}
```

## Improved styling with css

### Topography

<aside>
💡 How you are able to style and transform font.

</aside>

### Font-face in css

This how font-face is used in css with font family

```css
@font-face {
  font-family: 'MyParagraphFont';
  src: url('fonts/Roboto.woff2') format('woff2'),
       url('fonts/Roboto.woff') format('woff'),
       url('fonts/Roboto.ttf') format('truetype');
}
```

• The `@font-face` at-rule is used as the selector. It’s recommended to define the `@font-face` ruleset at the top of your CSS stylesheet.

## **Breadcrumbs** #

Date - 16/03/2024

<aside>
💡 Primary vs secondary

</aside>

Think about breadcrumbs 

### **What is primary vs secondary navigation?**

- The primary navigation system typically contains the most important links and buttons that need to be displayed on every single page of the site.
- Secondary navigation, or breadcrumb navigation, usually consists of a clickable list of pages or attributes that led to the current page. It can help users understand the extent of the site and also where they are currently

## **Benefit of using breadcrumbs**

Imagine using breadcrumbs as away of finding your way back easier on the site 

The decision to use breadcrumbs is a judgment call depending on the type, depth, and complexity of your site

When using bread crumbs they are separated with a `“>”` or a `“/“` symbol in the css styling.

Instead of having to manually add this to all of the breadcrumbs in our breadcrumb trail, we can use a CSS pseudo-element.

`.breadcrumb li+li::before` is the selector that we want! View the hint if you want more information about how this complicated selector works
In `styles.css`, find the selector (`.breadcrumb li+li::before`). Set the `content` property to “>” to place the greater than sign between each adjacent breadcrumb.

## **Where do Breadcrumbs Lead**

In the previous examples, if you clicked on any of the breadcrumbs, it wouldn’t take you to a new page. This is because we have set `href="#"`. With this value, a click on the link will cause the page to scroll to the top of the current page.
In a full site, these breadcrumbs would link to their respective pages. This is accomplished by setting the `href` property to the appropriate page

For example, if the breadcrumb list was:

`Fashion > Shoes > Flats > Brown`

and a user clicked on “Flats”, the breadcrumb list on that page should look like:

`Fashion > Shoes > Flats`

It would be confusing for a user if the categories or order of them changed like:

`Shoes > Shopping > Flats`

## **Breadcrumb Styles**

The example below makes use of a couple of CSS tricks to create an arrow effect. We’re using the `::before` and `::after` pseudo-elements to add filled rectangles (with empty content) before and after each list item:

```css
.breadcrumb li a::before, .breadcrumb li a::after {
  content: "";
  position: absolute;
  border-color: darkcyan;
  border-style: solid;
  border-width: 15px 5px;
}
.breadcrumb li a::before {
  left: -10px;
  border-left-color: transparent;
}
```

### Vocab

Location - based on hierarchical structure of site

Attribute - based on attributes of current page or item

path - unique to a user’s journey on the site

### Notes

- Important notes
- 

## Summary

- Use breadcrumbs to indicate where a user is and the extent of the site
- Breadcrumbs are implemented using unordered lists in HTML with custom CSS styling
- Three types of breadcrumbs exist:
    - **location** - based on hierarchical structure of site
- **attribute** - based on attributes of current page or item
- **path** - unique to a user’s journey on the site
- Path-based breadcrumbs can be confusing, only use if needed
- Ensure breadcrumbs will add value before adding to a site

---

## Flexbox - 1/1/2025

<aside>
💡

Flexbox is a layout method for arranging items in rows into smaller spaces.

</aside>

Flexbox’s purpose is to flexibly lay out a set of block or inline element in one dimension, flexbox vertically centres a block of content inside its parent. It will make all the children of a container take up an equal amount of the available width / height regardless of how much width / height is available. It will make all columns in a multiple-column layout adopt the same height even if they contain a different amount of content. 

### Flex box terminology

Flex container - definition

Flex item - definition

Align items - This property makes it possible to space flex items vertically

Flex grow -  Allows you to specify if items should grow to fill a container and also which items should grow proportionally more or less than others.

Flex shrink - Just like the flex grow  property flex - shrink can be used to specify which elements 

flex - basis - Another way to specify the width of a flex item is with the flex-basis property. flex-basis allows us to specify the width of an item before it stretches or shrinks

wrap - this wraps the child elements of a flex container that dont fit into a row will move down to the next line. 

wrap-reverse - the same functionality as wrap but the order is reversed 

no wrap - prevents the item from wrapping

align-items - is for aligning elements within a single row if the container is flexed and has multiple rows of content you can use align-content to space the rows from top to bottom. 

Flex - direction -  is used to define the direction in which the flex container's items are placed along the main axis

### Notes

- You need to specify what elements you want as flexible boxes when you do this the boxes will go side by side.
- Flex box uses values such as justify-content with flex-start / flex-end / flex-centre / space-around / space-between.
- Align items to baseline means the baseline of the content of each item will be aligned.
- Flex shorthand is a property that provides a way for specifying how elements stretch and shrink, while simplifying the css required
- You might not want the content to shrink to  fit its container.  But you might want to flex items to move to the next line. you can do this using the flex wrap property.

## Summary : Flexbox

1. `display: flex` changes an element to a block-level container with flex items inside of it.
2. `display: inline-flex` allows multiple flex containers to appear inline with each other.
3. `justify-content` is used to space items along the main axis.
4. `align-items` is used to space items along the cross axis.
5. `flex-grow` is used to specify how much space (and in what proportions) flex items absorb along the main axis.
6. `flex-shrink` is used to specify how much flex items shrink and in what proportions along the main axis.
7. `flex-basis` is used to specify the initial size of an element styled with `flex-grow` and/or `flex-shrink`.
8. `flex` is used to specify `flex-grow`, `flex-shrink`, and `flex-basis` in one declaration.
9. `flex-wrap` specifies that elements should shift along the cross axis if the flex container is not large enough.
10. `align-content` is used to space rows along the cross axis.
11. `flex-direction` is used to specify the main and cross axes.
12. `flex-flow` is used to specify `flex-wrap` and `flex-direction` in one declaration.
13. Flex containers can be nested inside of each other by declaring `display: flex` or `display: inline-flex` for children of flex containers.

---

# Intro to grids - 1/8/2025

<aside>
💡

Grid can be used to layout the entire web page. Flexbox is mainly used to position items in a one-dimensional layout, CSS grid is most used for two-dimensional lay outs  

</aside>

## Creating a Grid:

To set up a grid you need a grid container and grid items. The container acts as the parent element that contains grid items as the children and applies overarching styling and positioning to them. 

To make the html element know its a grid container you need to set the elements to the display property to one of two values ( grid - for a block -level grid) or ( inline-grid - for an inline grid ) 

## Creating Columns:

Grid by default contains only one column. So if you started to add an item it would put on a new row. To change this we need to explicitly define the number of rows and columns in our grid. 

You can define the columns of your grid by using the property ( grid-template-columns ). This property can create two changes first it defines the number of columns in the grid in this case there are two. The second sets the width of each column. 

## Creating Rows:

To create rows in the grid you need to specify the number and size of the rows, you can do this by using the grid-template-rows. For example [ grid-template-rows: 10% 20% 600px; ]

## Grid Template:

Grid template property can replace the previous two css properties. Both template-rows and template-columns

```css
.grid {
  display: grid;
  width: 1000px;
  height: 500px;
  grid-template: 200px 300px / 20% 10% 70%;
}
```

## Fraction:

<aside>
💡

You may already know about using different responsive units such as percentages ( % ), emS and remS. CSS grid has a new relative sizing unit - fr like fraction.

</aside>

From using the fr unit you can define the size of columns and rows as a fraction of the grid’s length and width. This unit was specifically created for CSS grid. When you use fr it makes it easier to prevent grid items from overlowing the boundaries  of the grid. Heres an example below:

```css
.grid {
  display: grid;
  width: 1000px;
  height: 400px;
  grid-template: 2fr 1fr 1fr / 1fr 3fr 1fr;
}
```

## Repeat

Some properties that define the number of rows and columns in a grid can take a function as a value. repeat() is one of these functions. The repeat() function was created specifically for CSS Grid. See the example below:

```css
.grid {
  display: grid;
  width: 300px;
  grid-template-columns: repeat(3, 100px);
}
```

The repeat function will duplicate the specifications for rows or columns a given number of times. Repeat is useful with the fr for example repeat ( 5, 1fr ) would split your table into five equal rows or columns.

The parameter of repeat( ) can have multiple values. for example:

```css
grid-template-columns: repeat(2, 20px 50px)
```

## Minmax

unless you define a size all of the grids by default have a fixed size some times you might want the grid to resize based on the size of your web browser. Heres an exmaple of using grid with min max:

```css
.grid {
  display: grid;
  grid-template-columns: 100px minmax(100px, 500px) 100px;
}
```

## Grid Gap

<aside>
💡

note that grid gap properties do not add space at the beginning or end of the grid

</aside>

CSS grid gap makes a space between each of the grids between every row and column in the grid

Heres an example of  using grid gap in css:

```css
.grid {
  display: grid;
  width: 320px;
  grid-template-columns: repeat(3, 1fr);
  column-gap: 10px;
}
```

## Grid items

<aside>
💡

A grid *container* contains grid *items,* a container has one grid item for each column, in each row, but you can style the grid items so that they will span multiple columns and/or rows

</aside>

heres an example of how youd use grid item that spans all five columns in a five column grid layout: 

```css
.item1 {
  grid-area: myArea;
}
.grid-container {
  grid-template-areas: 'myArea myArea myArea myArea myArea';
}
```

## Multiple Row Items

<aside>
💡

Using grid-row-start and grid-row-end you can make single grid items take up multiple rows.

</aside>

Heres an example of using multiple rows: 

```css
.item {
  grid-row-start: 1;
  grid-row-end: 3;
}
```

In this example, the HTML element of class `item` will take up two rows in the grid, rows 1 and 2. The values that `grid-row-start` and `grid-row-end` accept are *grid lines*.

## Grid Row

<aside>
💡

You can use grid-row as a short hand instead of start and end

</aside>

Heres a example of using grid-row for short hand 

```css
.item {
  grid-row: 4 / 6;
}
```

When an item spans multiple rows or columns using these properties, it will also include the `gap` if any exists.

## Grid Column

<aside>
💡

Grid-column works works identically to the row properties which allow a grid item to span multiple columns.

</aside>

Heres an example of using a grid-column:

```css
.item {
  grid-column: 4 / span 2;
}
```

This tells the item to begin in the column 4 and take up two columns of space.

## Grid Area

<aside>
💡

Grid area will set the starting and ending positions for both the rows and columns of an item

</aside>

Grid area tales four values separated by slashes keeping not of the order importance. This is how grid area interpret those values : grid-row-start / gird-column-start / grid-row-end / gird-row-end / see example below:

```css
.item {
  grid-area: 2 / 3 / 4 / span 5;
}
```

In the above example, the item will start on row `2` and end on row `4`, though the 4th row is not actually included, only rows `2` and `3`!

Vocab
• `grid-template-columns` - Sets column number and width
• `grid-template-rows` - Sets number and rows
• `grid-template` - is short hand property for both columns and rows
• `grid-template-area` - specifies named grid areas
• `row-gap` / `column-gap` / `gap` - adds spacing between each column in your your grid
• `grid-row-start` / `grid-row-end`  - defines how many rows an item will span
• `grid-area` - specifies a grid item's size and location within a grid

### Notes

- Important notes
- 

## Summary

- `grid-template-columns` defines the number and sizes of the columns of the grid
- `grid-template-rows` defines the number and sizes of the rows of the grid
- `grid-template` is a shorthand for defining both `grid-template-columns` and `grid-template-rows` in one line
- `row-gap` puts blank space between the rows of the grid
- `column-gap` puts blank space between the columns of the grid
- `gap` is a shorthand for defining both `row-gap` and `column-gap` in one line
- `grid-row-start` and `grid-row-end` makes elements span certain rows of the grid
- `grid-column-start` and `grid-column-end` makes elements span certain columns of the grid
- `grid-area` is a shorthand for `grid-row-start`, `grid-column-start`, `grid-row-end`, and `grid-column-end`, all in one line

---

## Advanced Grid - 1/10/2025

<aside>
💡

Grid-template-areas property allows you to name sections of your web page to use as values in the grid-template-row-start, grid-row-end, grid-column-start, grid-column-end, and grid-area which is declared on all containers.

</aside>

Heres an example of using grid to make a simple layout:

```css
/* html */
<div class="container">
  <header>Welcome!</header>
  <nav>Links!</nav>
  <section class="info">Info!</section>
  <section class="services">Services!</section>
  <footer>Contact us!</footer>
</div>
/* css */
.container {
  display: grid;
  max-width: 900px;
  position: relative;
  margin: auto;
  grid-template-areas: "header header"
                       "nav nav" 
                       "info services"
                       "footer footer";
  grid-template-rows: 300px 120px 800px 120px;
  grid-template-columns: 1fr 3fr; 
}

header {
  grid-area: header;
} 

nav {
  grid-area: nav;
} 

.info {
  grid-area: info;
} 

.services {
  grid-area: services;
}

footer {
  grid-area: footer;
} 
```

Output from the code above!

![image.png](image.png)

## Overlapping elements

<aside>
💡

CSS can do a powerful feature that allows css grid layout to easily overlap elements

</aside>

overlapping elements is generally done with using the grid-area property with grid row names, just remember that grud-area will set the starting and ending postiong for both the rows and columns of an item. 

Heres an example with some code.

```css
/* HTML */
<div class="container">
  <div class="info">Info!</div> 
  <img src="#" />
  <div class="services">Services!</div>
</div>

/* CSS */
.container {
  display: grid;
  grid-template: repeat(8, 200px) / repeat(6, 100px);
}

.info {
  grid-area: 1 / 1 / 9 / 4;
}

.services {
  grid-area: 1 / 4 / 9 / 7;
}

img {
  grid-area: 2 / 3 / 5 / 5;
  z-index: 5;
}

```

Heres an example of using grid with overlapping elements 

```css
/* HTML */
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <title>Grid Stuff</title>
  <link rel="stylesheet" href="style.css" />
</head>

<body>
  <div class="container">
    <header>
      <h1>Header</h1>
    </header>
    <nav>
      <h1>Nav</h1>
    </nav>
    <section class="left">
      <h2>Left</h2>
    </section>
    <div class="overlap">
      <h3>Overlap!</h3>
    </div>
    <section class="right">
      <h2>Right</h2>
    </section>
    <footer>
      <h1>Footer</h1>
    </footer>
  </div>
</body>
</html>

/* CSS */
.container {
  display: grid;
  max-width: 900px;
  position: relative;
  margin: auto;
  gap: 10px;
  grid-template: repeat(12, 1fr) / repeat(6, 1fr);
}

h1, h2, h3 {
  font-family: monospace;
  text-align: center;
}

header {
  background-color: dodgerblue;
  grid-area: 1 / 1 / 3 / 7;
}

nav {
  background-color: beige;
  grid-area: 3 / 1 / 4 / 7;
}

.left {
  background-color: dodgerblue;
  grid-area: 4 / 1 / 9 / 5 ;
}

.right {
  background-color: beige;
  grid-area: 4 / 5 / 9 / 7;
}

.overlap {
  background-color: lightcoral;
  grid-area: 6 / 4 / 8 / 6;
  z-index: 5;
}

footer {
  background-color: dodgerblue;
  grid-area: 9 / 1 / 13 / 7;
}
```

Heres an example of how the above code works on a page 

![image.png](image%201.png)

## Justify-Items

<aside>
💡

There are two axes in a grid layout - the column or block axis and the inline or row axis.

</aside>

In grid the column axis stretches from top to bottom across the web page. The row axis stretches from left to right across the web page.

Vocab 
• `start` — aligns grid items to the left side of the grid area
• `end` — **aligns grid items to the right side of the grid area**
• `center` — aligns grid items to the center of the grid area
• `stretch` — stretches all items to fill the grid area

### Notes

- `justify-items` aligns grid items along the inline (row) axis within their grid area.
- Can take `inherit`, `initial`, or `unset` as values
- The default is `stretch`, which makes items fill the grid cell width.

An example of using justify-items in code

```css
/* HTML */
<main>
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
</main>
/* CSS  */
main {
  display: grid;
  grid-template-columns: repeat(3, 400px);
  justify-items: center;
}

```

---

## Justify-content

<aside>
💡

Justify-content is used to position the entire grid along the row axis. This property is declared on grid containers.

</aside>

An example of using justify-content in regular css

```css
/* HTML */
<main>
  <div class="left">Left</div>
  <div class="right">Right</div>
</main>
/* CSS  */
main {
  display: grid;
  width: 1000px;
  grid-template-columns: 300px 300px;
  grid-template-areas: "left right"; 
  justify-content: center;
}

```

### Vocab

Start  - aligns the grid to the left side of the grid container

End - aligns the grid to the right side of the grid container

Center - centers the grid horizontally in the grid container

Stretch - stretches the grid items to increase the size of the grid to expand horizontally across the container

Space-around - includes an equal amount of space on each side of a grid element, resulting in double the amount of space between elements as there is before the first and after the last element

Space-between - includes an equal amount of space between grid items and no space at either end

Space-evenly - places an even amount of space between grid items and at either end

### Notes

- There are several other values that justify-content accepts that you can look at
- 

---

## Align Items

<aside>
💡

 align-items is a property that positions grid items along the block, or column axis , This means that it positions items from top to bottom.

</aside>

The narrower left column is for recording keywords, questions, and recall prompts. The right column is for your actual notes taken during a lecture or class.

### Vocab

start  - aligns grid items to the top side of the grid area

end - ligns grid items to the bottom side of the grid area

center - aligns grid items to the center of the grid area

stretch - stretches all items to fill the grid area

### Notes

- This property is declared on grid containers.
- There are several other values that `align-items` accepts
- The default value is 'stretch', which ensures grid items fill their entire grid area vertically

Heres an example of using align-items in css code

```css
/* HTML */
<main>
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
</main>
/* CSS  */
main {
  display: grid;
  grid-template-rows: repeat(3, 400px);
  align-items: center;
}

```

---

## Align Content

<aside>
💡

`align-content` positions the rows along the column axis, or from top to bottom

</aside>

For `align-content` to work, the grid container must have extra vertical space. If the grid tracks already fill the container, changing `align-content` won't produce any visual difference.

### Vocab

`start` — aligns the grid to the top of the grid container

`end` — aligns the grid to the bottom of the grid container

`center` — centres the grid vertically in the grid container

`stretch` — stretches the grid items to increase the size of the grid to expand vertically across the container

`space-around` — includes an equal amount of space on each side of a grid element, resulting in double the amount of space between elements as there is before the first and after the last element

`space-between` — includes an equal amount of space between grid items and no space at either end

### Notes

- This property is particularly useful for grid layouts that need to adapt to different screen sizes or content amounts
- The default value is 'stretch', which makes the grid fill the available container space
- When using 'space-around' or 'space-between', ensure there's enough space in the container for the spacing to be visible

---

## Justify Self and Align Self

<aside>
💡

The `justify-items` and `align-items` properties specify how all grid items contained within a single container will position themselves along the row and column axes, respectively.

</aside>

The justify-self specifies how an individual element is positioned to the row axis this property will override justify-items for any item on which is declared,

Align-self specifies an individual element also to the column axis this property will override align-items for any item on which it s declared.

### Vocab

`start` — positions grid items on the left side/top of the grid area

`end` — positions grid items on the right side/bottom of the grid area

`center` — positions grid items on the centre of the grid area

`stretch` — positions grid items to fill the grid area (default)

### Notes

- The justify-self and align-self properties give you precise control over individual grid item positioning, unlike their container-level counterparts
- These properties are particularly useful when you need to create exceptions to the overall grid alignment pattern
- Both properties accept the same values and follow similar behavior patterns, just on different axes

---

## Implicit vs. Explicit Grid

<aside>
💡

implicit grid in CSS is automatically generated vs explicit grid in CSS is defined by the developer

</aside>

## Key Concepts

- **Grid Elements**: Grid elements are defined using various properties to specify their dimensions and quantities.
- **Static vs. Dynamic Content**:
    - **Static Content**: Works well for fixed layouts, like a business landing page that displays a specific amount of information.
    - **Dynamic Content**: Challenges arise when the amount of information displayed is unknown, such as in online shopping scenarios.

## Implicit Grid

- **Definition**: The implicit grid is an algorithm in CSS Grid that automatically manages the placement of elements when there are more items than the defined grid can accommodate.
- **Default Behavior**:
    - Items fill rows first.
    - New rows are created as needed.
    - Each new row adjusts its height to fit the content it contains.

## Example Scenario

- If a developer sets a grid with **3 columns and 5 rows** (totaling 15 items) but receives **30 search results**, the implicit grid will:
    - Automatically create additional rows to accommodate the extra items.

---

## Grid auto Rows and Grid Auto Columns

<aside>
💡

grid-auto-rows specifies the height of implicitly added grid rows. grid-auto-columns specifies the width of implicitly added grid columns

</aside>

`grid-auto-rows` and `grid-auto-columns` accept the same values as their explicit counterparts,
`grid-template-rows` and `grid-template-columns`:

```css
/* HTML */
<body>
  <div>Part 1</div>   
  <div>Part 2</div>
  <div>Part 3</div>
  <div>Part 4</div>
  <div>Part 5</div>
</body>
/* CSS */
body {
  display: grid;
  grid: repeat(2, 100px) / repeat(2, 150px); 
  grid-auto-rows: 50px;
}
```

### Vocab

Pixels- ( px )

Percentages - ( % )

fractions  - ( fr )

repeat () - function

### Notes

- These units (px, %, fr, repeat()) are fundamental for creating flexible and responsive grid layouts
- Pixels provide precise control but are static, while percentages and fractions offer more fluid responsiveness
- The repeat() function helps create consistent grid patterns while reducing code repetition

---

## Grid Auto Flow

<aside>
💡

You can specify the order in which the rows and columns are rendered.

</aside>

`grid-auto-flow` specifies whether new elements should be added to rows or columns, and is declared on grid containers.

You can pair `row` or `column` with `dense`, like this: `grid-auto-flow: row dense;`.
Here is an example of using `grid-auto-flow: column;` with the `grid-auto-columns` property:

```css
/* HTML */
<body>
    <div class='box'>Part 1</div>   
    <div class='box'>Part 2</div>
    <div class='box'>Part 3</div>
    <div class='box'>Part 4</div>
    <div class='box'>Part 5</div>
</body>
/* CSS */
body {
  display: grid;
  gap: 5px;
  grid: repeat(2, 100px) / repeat(2, 150px);
  grid-auto-rows: 45px;
  grid-auto-columns: 65px;
  grid-auto-flow: column;
}
```

This creates the following on a page

![image.png](image%202.png)

### Vocab

• `row` — specifies the new elements should fill rows from left to right and create new rows when there are too many elements (default)
• `column` — specifies the new elements should fill columns from top to bottom and create new columns when there are too many elements

`dense` — this keyword invokes an [algorithm](https://www.codecademy.com/resources/docs/general/algorithm) that attempts to fill holes earlier in the grid layout if smaller elements are added

### Important Notes

- `grid-auto-flow` determines whether new elements are placed in rows or columns in the grid layout.
- The default value is `row`, meaning elements are added from left to right and new rows are created as needed.
- Adding the `dense` keyword allows the algorithm to fill gaps in the grid by placing smaller elements into empty spaces, optimizing the layout.

## Summary:

- `grid-template-areas` specifies grid named grid areas.
- grid layouts are two-dimensional: they have a row, or inline, axis and a column, or block, axis.
- `justify-items` specifies how individual elements should spread across the row axis
- `justify-content` specifies how groups of elements should spread across the row axis
- `justify-self` specifies how a single element should position itself with respect to the row axis
- `align-items` specifies how individual elements should spread across the column axis
- `align-content` specifies how groups of elements should spread across the column axis
- `align-self` specifies how a single element should position itself with respect to the column axis
- `grid-auto-rows` specifies the height of rows added implicitly to the grid
- `grid-auto-columns` specifies the width of columns added implicitly to the grid
- `grid-auto-flow` specifies in which direction implicit elements should be created

---

## Sizing Elements

<aside>
💡

Sizing Elements : **Relative Measurements refers to the ability of a website resize and recognize its content based on the size of other content on the website and the size of the screen the website is being viewed on.**

</aside>

Responsive design normally uses units of px  / rem / em / vh / vw. These relative units allow elements to scale proportionally based on screen size or parent element dimensions, making layouts more flexible and adaptable across different devices.

## Rem:

Rem Stands for root em. it acts similar to em but instead of checking parent elements to font, it checks the root element.

Below is an example of using em and px for font-size: 

```css
.heading {
  font-size: 2em;
}
/* Assuming the default font size is 16 pixels, then the font size of the heading element will be 32 pixels. */
.splash-section {
  font-size: 18px;
}

.splash-section h1 {
  font-size: 1.5em;
}
/* The example above shows how to use ems without relying on the default font size of the browser. Instead, a base font size (18px) is defined for all text within the splash-section element. The second CSS rule will set the font size of all h1 elements inside of splash-section relative to the base font of splash-section (18 pixels). The resulting font size of h1 elements will be 27 pixels.*/

```

## Percentages: Height & Width

Percentages are often used to size box-model values, such as width height padding and border and margins, they can also be used to set positioning properties ( top, bottom, left, right )

## Width: Min & Max

Websites can lose their integrity when they become too small or large. To solve this issue you can use certain properties such as min-width and max-width

Heres an example of using the properties with a paragraph element

```css
p {
  min-width: 300px;
  max-width: 600px;
}
```

## Height: Min & Max

You can also set the limit for hight with min and max properties such as min-height and max-height

```css
p {
  min-height: 150px;
  max-height: 300px;
}
```

## Scaling Images and Videos

Websites contain a lot of media such as images and videos it is important make sure that they are scaled properly so that users can correctly view it.

Heres an example of how you would scale media in a div with a class of .container

```css
.container {
  width: 50%;
  height: 200px;
  overflow: hidden;
}

.container img {
  max-width: 100%;
  height: auto;
  display: block;
}
```

### Vocab

pixels - or (px) is a absolute unit of measurement representing a fixed number of screen pixels.

rem - is a relative unit of measurement based on the font size of the root element.

em -  is a relative unit of measurement based on the font size of the current element or its parent, depending on context.

vh  - is a relative unit representing 1% of the viewport height.

vw - is a relative unit representing 1% of the viewport width. 

`min-width` — ensures a minimum width for an element.

`max-width` — ensures a maximum width for an element.

### Notes

- Comprehensive guide to CSS covering styling methods, selectors, specificity, box model, flexbox, grid layouts, responsive design, and advanced techniques like pseudo-classes, breadcrumbs, and implicit/explicit grids.

### **Review: Relative Measurements**

1 min

Great work! You learned how to size elements on a website relative to other elements on the page.

Let’s review what you learned:

- Content on a website can be sized relative to other elements on the page using *relative measurements*.
- The unit of `em` sizes font relative to the font size of a parent element.
- The unit of `rem` sizes font relative to the font size of a root element. That root element is the `<html>` element.
- Percentages are commonly used to size box-model features, like the width, height, padding, or margin of an element.
- When percentages are used to size width and height, child elements will be sized relative to the dimensions of their parent (remember that parent dimensions must first be set).
- Percentages can be used to set padding and margin. Horizontal and vertical padding and margin are set relative to the width of a parent element.
- The minimum and maximum width of elements can be set using `min-width` and `max-width`.
- The minimum and maximum height of elements can be set using `min-height` and `max-height`.
- When the height of an image or video is set, then its width can be set to `auto` so that the media scales proportionally. Reversing these two properties and values will also achieve the same result.
- A background image of an HTML element will scale proportionally when its `background-size` property is set to `cover`.

---

## Responsive Design Media Queries - 01/23/2025

<aside>
💡

If a website isnt responsive it may look indecipherable on certain devices. This normally occurs on smaller screens, such as phones.

</aside>

## View port meta tag

The view port meta tag is the total viewable area for a user, This area varies depending on device. The view port is smaller on mobile device and large on desktop. The meta tag is used to instruct the browser on how render the webpages scale and dimensions for example if a site is 960px and the device is 320px wide, adding the viewport meta tag will squish the content down until it is 320px - there is no  need for the user to zoom out and view the whole page.

Heres an example of what the Meta tag looks like in html code

```html
<!DOCTYPE html> 
<html lang="en"> 
  <head> 
    ...
    <meta name="viewport" content="width=device-width, initial-scale=1">
    ...
  </head> 

```

## Media queries

<aside>
💡

Media queries are used to adapt a websites content to different screen sizes with media queries, CSS can detect the size of the current  screen and apply different css styles depending on the width of the screen.

</aside>

Heres an example of using a media query in css

```css
@media only screen and (max-width: 480px) {
  body {
    font-size: 12px;
  }
}
/* this code will make the bodys font-size 12px if the max-wdith is 480px */
```

The media query defines a rule for screens smaller than 480 pixels (approximately the width of many smartphones in [landscape](https://en.wikipedia.org/wiki/Page_orientation) orientation).

This is another example of using the media query to make the page-title for the css be 270px  when the screen is a size of 480px.

```css
@media only screen and (max-width : 480px) { 
  .page-title {
    width: 270px;
  }
}
```

## Range

<aside>
💡

Specific screen sizes can be targeted by setting multiple width and heigh media features. 

</aside>

By using multiple widths and heights, a range can be set for a media query. 

```css
@media only screen and (min-width: 320px) and (max-width: 480px) {
    /* ruleset for 320px - 480px */
}
```

Heres an example of using multiple media queries

```css
/* The first media query in the example above will apply CSS rules 
when the size of the screen meets or exceeds 320 pixels */
@media only screen and (min-width: 320px) { 
    /* ruleset for >= 320px */
}

/* The second media query will then apply CSS rules when the size of the screen meets or exceeds 480 pixels,
meaning that it can override CSS rules present in the first media query or 
apply additional CSS rules that are not already present in the first. */
@media only screen and (min-width: 480px) { 
    /* ruleset for >= 480px */
}

```

## Dots Per Inch (DPI)

Another media feature you can target is screen resolution. Many times you would want to supply higher quality media ( images, video etc ). only to users with screens that can support high resolution media. Targeting screen resolution also helps users avoid downloading high res images at their screen may not be able to properly display.

To target by resolution you can use the min-resolution and max-resolution media features as shown bellow.

```css
/*These media features accept a resolution value in either dots per inch ( dpi ) or dots per centimeter 
( dcp ) */
@media only screen and (min-resolution: 300dpi) {
    /* CSS for high resolution screens */
    .logo {
    background-image: url("../img/spaceship@2x.png");
  }
}

```

## And Operator

<aside>
💡

Before we covered multiple media features of the same type in one media query by using the and operator. It allowed you to create a range by using min-width and max-width in the same media query

</aside>

Here is an example :

```css
@media only screen and (max-width: 480px) and (min-resolution: 300dpi) {
    /* CSS ruleset */
}
```

## Comma Separated List

<aside>
💡

Media features can be seperated in a comma sperated list.

</aside>

Here is an example of how you would separate media features in a comma separated list.

```css
@media only screen and (min-width: 480px), (orientation: landscape) {
    /* CSS ruleset */
}
```

Note that the second media feature is `orientation`. The `orientation` media feature detects if the page has more width than height. If a page is wider, it’s considered `landscape`, and if a page is taller, it’s considered `portrait`.

## Breakpoints

<aside>
💡

The points at which media queries are set are called break points.

</aside>

Breakpoints are the screen sizes at which your web page does not appear properly. Below is an example if you want to target tablets that are in landscape orientation you can create them like this.

```css
@media only screen and (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    /* CSS ruleset */
}
```

### Vocab

@media - This keyword begins a media query rule and instructs the CSS compiler on how parse the rest of the rule.

Only Screen -  This indicates what type of devices should use this rule in early attempts to target different devices.

And ( max-width : 480px ) - this part of the rule is called a media feature instructs the css compiler to apply the css styles to devices with a width of 480 pixels or smaller.

CSS rules are nested instead of the media query’s curly braces. The rules will be applied when the media query is met.In the example above, the text in the `body` element is set to a `font-size` of `12px` when the user’s screen is less than 480px.

### Notes

- the `name="viewport"` attribute: tells the browser to display the web page at the same width as its screen
- he `content` attribute: defines the values for the `<meta>` tag, including `width` and `initial-scale`
- the `width=device-width` key-value pair: controls the size of the viewport in which it sets the width of the viewport to equal the width of the device
- the `initial-scale=1` key-value pair: sets the initial zoom level (Read more about scale at [MDN’s viewport documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag#viewport_basics))

## **Summary : Media Queries**

Incredible work! You learned how to change the way a website appears on different screens with media queries and breakpoints

Throughout this lesson, you learned:

- When a website responds to the size of the screen it’s viewed on, it’s called a *responsive* website.
- You can write *media queries* to help with different screen sizes.
- Adding the viewport `<meta>` tag to our code allows us to control the width and scaling of the viewport so that it’s sized and scaled correctly on all devices.
- Media queries require *media features*. Media features are the conditions that must be met to render the CSS within a media query.
- Media features can detect many aspects of a user’s browser, including the screen’s width, height, resolution, orientation, and more.
- The `and` operator requires multiple media features to be true at once.
- A comma separated list of media features only requires one media feature to be true for the code within to be applied.
- The best practice for identifying where media queries should be set is by resizing the browser to determine where the content naturally breaks. Natural breakpoints are found by resizing the browser.

---