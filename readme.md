# [COMPSCI235] Lab Report 2

## HTML
HTML is the abbreviation of Hypertext Markup Language, which is `"Hypertext Markup Language"` Note that it is a markup language, **`NOT`** a programming language.
- HyperText: a structured text
- Markup language: a systematic grammar for marking up text

Here is the sample code:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>

        <h1>This is a Heading</h1>
        <p>This is a paragraph.</p>

    </body>
</html>
```

### Tags
HTML tags are all paired and in a `"Nested"` structure.
The symbol surrounded by `< >` is the `"tag"` of the markup language such as HTML. The tag generally needs to have a clear start and end to surround a piece of text:`<head></head>`
- Headings:` h1, h2, h3, h4, h5, h6`

- Text paragraph:` p`
    ```html
    <p>Welcome to Compsci235!</p>
    ```
- Emphasis:` em, strong`
    ```html
    <em>Italic</em>
    ```
    ```html
    <strong>Bold</strong>
    ```
- List:` ul, ol, li`
    ```html
    <ul><!-- unordered list -->
        <li>Working Directory</li>
        <li>Staging Area</li>
        <li>Repository</li>
    </ul>
    ```
    ```html
    <ol><!-- ordered list -->
        <li>Working Directory</li>
        <li>Staging Area</li>
        <li>Repository</li>
    </ol>
    ```

- newline:` br`
    ```html
    <br> <!-- new line -->
    <br/> <!-- new line -->
    ```
- Horizontal line:` hr`
    ```html
    <hr><!-- create a line like this —————————————————— -->
    ```
- Hyperlink: `a `
    ```html
    <a href="https://www.auckland.ac.nz">UoA</a>
    ```

- Image:` img`
    ```html
     <img src="source_URL" alt="Text when image cannot load">
    ```
- Area: `div, span`
    ```html
    <div style="color:#0000FF">
        <h3>here is title in div element</h3>
        <p>here is text in div element</p>
    </div>
    ```
    ```html
    <p>The text will become <span style="color:blue">blue </span> in span element</p>
    
    ```
- Table: `table, tr, th, td`
    ```html
    <!-- table -->
    <table border="1">
        <tr>
            <th>Month</th><!-- row 1 column 1 -->
            <th>Savings</th><!-- row 1 column 2 -->
        </tr>
        <tr>
            <td>January</td><!-- row 2 column 1 -->
            <td>$100</td><!-- row 2 column 2 -->
        </tr>
        <tr>
            <td>February</td><!-- row 3 column 1 -->
            <td>$80</td><!-- row 3 column 2 -->
        </tr>
    </table>
    ```
- Form:` form, label, input`
    ```html
    <form action="demo_form.php" method="get">
        First name: <input type="text" name="fname"><br>
        Last name: <input type="text" name="lname"><br>
        <input type="submit" value="submit">
    </form>
    ```
    ```html
    <form action="demo_form.php" method="get">
        <label for="male">Male</label>
        <input type="radio" name="sex" id="male" value="male"><br>
        <label for="female">Female</label>
        <input type="radio" name="sex" id="female" value="female"><br><br>
        <input type="submit" value="submit">
    </form>
    ```
    
<div style="page-break-after: always"></div>

## CSS
`Cascading Style Sheets` (css), is a computer language used to add styles (fonts, spacing, colors, etc.) to structured documents such as HTML documents or XML applications.

```css
h1 {
    color: red;
}
```

Form the above, `h1` is the selector, `color` are the attributes, and `red` is the values.

The `selector` defines who your style has an effect on. It may correspond to the HTML tag name or the class and id attributes.

Note that CSS is specified with a colon (**`:`**) rather than an equal sign (**`=`**). 
Separate each declaration with a semicolon (**`;`**)

### Common Attributes
There are some common attributes:
- Background
    ```css
    background-image:url('img_tree.png');
    background-repeat:no-repeat;
    background-position:right top;
    background-attachment:fixed;

    background:#ffffff url('http://static.runoob.com/images/mix/img_tree.png') no-repeat right top;
    ```
- font
    ```css
    font:italic bold 12px/30px Georgia, serif;

    font-size:40px;
    font-style:italic;
    font-weight:bold;
    font-variant:small-caps;
    font-family:"Times New Roman",Georgia,Serif;
    ```
- margin and padding
    ```css
    margin:25px 50px 75px 100px;
    margin:25px 50px 75px;
    padding:25px 50px;
    padding:25px;

    margin-top:100px;
    margin-bottom:100px;
    padding-right:50px;
    padding-left:50px;
    ```
- height and width
    ```css
    height:50px;
    width:100px
    ```
- position
    ```css
    position:fixed;
    top:30px;
    right:5px;
    ```

<div style="page-break-after: always"></div>

## Bootstrap
`Bootstrap` is a front-end framework written in HTML, CSS and JavaScript. It makes the `layout of the website` automatically adapt to the screen size. It does a set of website `infrastructure` in advance, develops on the   `basis of the framework`, and does not need to worry about trivial settings.

1. Basic Structure:
    - Provides a `basic` structure with grid system, link styles, background.

2. CSS:
    - Comes with `global CSS settings`, defining basic HTML element styles, extensible classes, and an advanced grid system.

3. Components: 
    - Contains multiple reusable `components` for creating images, dropdown menus, navigation, alert boxes, popovers, and more.

4. JavaScript plugins: 
    - Contains several custom `jQuery plugins`. All plugins can be included directly, or they can be included one by one.


<div style="page-break-after: always"></div>

## Lab Question
1. What is HTML and what are HTML tags?
    - HTML -- `Hypertext Markup Language` is the language for creating Web pages. 
        - HyperText: a structured text
        - Markup language: a systematic grammar for marking up text
    - HTML tags use for define how web content is to be presented. HTML elements label pieces of content. For example,   `<h1>...</h1>`is heading, `<p></p>` is paragraph.

2. How many levels of heading does an HTML have?
    - there are total 6 levels.
        - h1, h2, h3, h4, h5, h6

3. Here is a HTML page that has a syntax error: 
    ```
    <h3>This is my awesome title!</h1>
    ```
    What does it look like in a rendered page?
    - Here is the example with `<h3></h1>`
        <h3>This is my awesome title!</h1>
        
        Here is the example with `###`
        ### This is my awesome title!

        The example with `<h3></h1>` looks the same with the title using ###
    
4. How to add a comment to a HTML page?
    - Add comment start with `<!--` and end with `-->` 
        - e.g. `<!-- Add comment here -->`
5. Name 3 commonly used CSS selectors.
    - class Selector
        - e.g. `.intro` selects all elements with `class="intro"`
    - id Selector
        - `#firstname` selects the element with `id="firstname"`
    - elementelement Selector
        - e.g. `p` selects all `<p> `elements
    
6. Whatʼs the difference between padding and margin in CSS?
    - `margin` is the space around an element's border
    -  `padding` is the space between an element's border and the element's content

7. What units can you use when defining a padding? (Name at least 2.) 
    - `px`
        - e.g. padding: 10px 50px 30px 0;
    - `%`
        - e.g. padding: 10% 0;
    - `em`
        - e.g. padding: 1em;