---
layout: layout.liquid
pageTitle: LEARN CSS
---
<h1 class="centered_para">Explore CSS</h1>
<div class="flex-container">
  <div class="resizing"><a href="#selector-start"><strong>Selectors</strong></a></div>
  <div class="resizing"><a href="#css-funcs"><strong>Functions</strong></a></div>
  <div class="resizing"><a href="#fonts-info"><strong>Fonts</strong></a></div>  
  <div class="resizing"><a href="#boxmodel"><strong>Box Model</strong></a></div>
  <div class="resizing"><a href="/tutorials/html_css_cheats"><strong>Cheats</strong></a></div>
</div>

<div class="example">
  <header>
    <strong>CSS: general</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <strong>CSS</strong> is Cascading Style Sheets.
    <ul>
    <li>CSS describes how HTML elements are to be displayed on screen, paper, or in other media</li>
    <li>External stylesheets are stored in CSS files</li><br>    
    <li>CSS syntax:</li>
    <li>A CSS rule-set consists of a selector and a declaration block</li><br>
    <li><code>p {color: red;text-align: center;}</code></li>
    <li><p>"p"-selector; "color: red" and "text-align: center" - declarations</li>
    <li>Each declaration includes a CSS property name and a value, separated by a colon.</li>
    </ul>
    External styles are defined within the <link> element, inside the <head> section of an HTML page:</br>
    <code>&ltlink rel="stylesheet" type="text/css" href="mystyle.css"&gt</code>
    </div>

  </main>
</div>

<div class="example">
  <header id="selector-start">
    <strong>Selectors</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    CSS selectors are used to "find" (or select) the HTML elements you want to style.<br>
    We can divide CSS selectors into five categories:
    <ul>
    <li>Simple selectors (select elements based on name, id, class</li>
    <li>Combinator selectors (select elements based on a specific relationship between them)</li>    
    <li>Pseudo-class selectors (select elements based on a certain state)</li>
    <li>Pseudo-elements selectors (select and style a part of an element)</li>
    <li>Attribute selectors (select elements based on an attribute or attribute value)</li>
    </ul>    
    <table id="selectors">
  <tr>
    <th>Selector</th>
    <th>Example</th>
    <th>Example description</th>
  </tr>
  <tr>
    <td>.class</td>
    <td>.intro</td>
    <td>Selects all elements with class="intro"</td>
  </tr>
  <tr>
    <td>.class1.class2</td>
    <td>.name1.name2</td>
    <td>Selects all elements with both name1 and name2 set within its class attribute</td>
  </tr>
  <tr>
    <td>#id</td>
    <td>#firstname</td>
    <td>Selects the element with id="firstname"</td>
  </tr>
  <tr>
    <td>*</td>
    <td>*</td>
    <td>Selects all elements</td>
  </tr>
  <tr>
    <td>element</td>
    <td>p</td>
    <td>Selects all &ltp&gt elements</td>
  </tr>
  <tr>
    <td>element.class</td>
    <td>p.intro</td>
    <td>Selects all &ltp&gt elements with class="intro"</td>
  </tr>
  <tr>
    <td>element, element</td>
    <td>div, p</td>
    <td>Selects all &ltdiv&gt elements and all &ltp&gt elements</td>
  </tr>
  <tr>
    <td>element element</td>
    <td>div p</td>
    <td>Selects all &ltp&gt elements inside &ltdiv&gt elements</td>
  </tr>
  <tr>
    <td>element>element</td>
    <td>div > p</td>
    <td>Selects all &ltp&gt elements where the parent is a &ltdiv&gt element</td>
  </tr>
  <tr>
    <td>:hover</td>
    <td>a:hover</td>
    <td>Selects links on mouse over</td>
  </tr>
  <tr>
  <td>
  +many others
  </td>
</table>
    </div>

  </main>
</div>

<div class="example">
  <header id="css-funcs">
    <strong>Functions</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    CSS functions are used as a value for various CSS properties.<br>
    <table id="selectors">
  <tr>
    <th>Function</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>attr() - Returns the value of an attribute of the selected element </td>
    <td><code>a:after {
  content:"("attr(href)")";
}</code></td>
    <td>The following example inserts the value of the href attribute in parenthesis after each link</td>
  </tr>
  <tr>
    <td>calc() - Allows you to perform calculations to determine CSS property values</td>
    <td><code>#div1 {<br>
  position: absolute;<br>
  left: 50px;<br>
  width: calc(100% - 100px);<br>
  border: 1px solid black;<br>
  background-color: yellow;<br>
  padding: 5px;<br>
  text-align: center;<br>
}</code></td>
    <td>Use calc() to calculate the width of a div element</td>
  </tr>
  <tr>
    <td>linear-gradient() - Sets a linear gradient as the background image. Define at least two colors (top to bottom)</td>
    <td><code>#grad {
  background-image: linear-gradient(red, yellow, blue);
}</code></td>
    <td id="grad">This linear gradient starts at the top. It starts red, transitioning to yellow, then to blue</td>
  </tr>
  <tr>
    <td>radial-gradient() - Sets a radial gradient as the background image. Define at least two colors (center to edges)</td>
    <td><code>#radgrad {
  background-image: radial-gradient(red, yellow, blue);
}</code>
</td>
    <td id="radgrad">A radial gradient with evenly spaced color stops</td>
  </tr>
  <tr>
    <td>rgb() - defines colors using the Red-Green-Blue model (RGB)</td>
    <td><code>#rgbfunc {background-color:rgb(255,0,0);} /* red */</code></td>
    <td id="rgbfunc">Define different RGB colors</td>
  </tr>
  <tr>
    <td>hsl() - defines colors using the Hue-Saturation-Lightness model (HSL)</td>
    <td><code>#hslfunc {background-color:hsl(120,100%,75%);}</code></td>
    <td id="hslfunc">Define different HSL colors</td>
  </tr>
  <tr>
    <td>var() - Inserts the value of a custom property</td>
    <td><code>:root {
  --main-bg-color: coral;
}<br>
#div1 {
  background-color: var(--main-bg-color);
}</code>
</td>
    <td>First define a custom property named "--main-bg-color", then use the var() function to insert the value of the custom property later in the style sheet</td>
  </tr>
</table>
    </div>

  </main>
</div>


<div class="example">
  <header id="fonts-info">
    <strong>Fonts</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice"><p>
    The <code>font-family</code> property should hold several font names as a "fallback" system, to ensure maximum compatibility between browsers/operating systems. If the browser does not support the first font, it tries the next font.<br>
    You can also use Google fonts by &ltlink&gting them as style in head.<br>
    Start with the font you want, and end with a generic family, to let the browser pick a similar font in the generic family, if no other fonts are available:</p>
    <code> p {
  font-family: "Times New Roman", Times, serif;
}</code> 
    <table id="selectors">
  <tr>
    <th>Font-family</th>
    <th>Example-code</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>Georgia, serif</td>
    <td><code>#georgia {
	font-family: Georgia, serif;
  }</code>
  </td>
    <td id="georgia">This is text</td>
  </tr>
  <tr>
    <td>Arial, Helvetica, sans-serif</td>
    <td><code>#arial {
	font-family: Arial, Helvetica, sans-serif;
  }</code></td>
    <td id="arial">This is text</td>
  </tr>
  <tr>
    <td>"Lucida Console", Monaco, monospace</td>
    <td><code> #lucida {
	font-family: "Lucida Console", Monaco, monospace;
  }</code>
  </td>
    <td id="lucida">This is text</td>
  </tr>
</table>
    </div>
  </main>
</div>


<div class="example">
  <header>
    <strong>Borders</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice"><p>
    The CSS <code>border</code> properties allow you to specify the style, width, and color of an element's border.<br>
    The <code>border-color</code> property is used to set the color of the four borders.<br>
    The <code>border-width</code> property specifies the width of the four borders.<br>
    The <code>border-radius</code> property is used to add rounded borders to an element
    <table id="selectors">
  <tr>
    <th>Border properties</th>
    <th>Example-code</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>dotted</td>
    <td><code>#dotted-b {border-style: dotted; border-color: blue;}</code>
  </td>
    <td><p id="dotted-b">This is text</p></td>
  </tr>
  <tr>
    <td>dashed </td>
    <td><code>#dashed-b {border-style: dashed;border-left: 6px solid red;}</code></td>
    <td><p id="dashed-b">This is text</p></td>
  </tr>
  <tr>
    <td>solid</td>
    <td><code> #solid-b {border-style: solid; border-radius: 10px;}</code>
  </td>
    <td><p id="solid-b">This is text</p></td>
  </tr>
</table>
    </div>
  </main>
</div>

<div class="example">
  <header id="boxmodel">
    <strong>Box model</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice"><p>
    All HTML elements can be considered as boxes. In CSS, the term "box model" is used when talking about design and layout.<br>
    The CSS box model is essentially a box that wraps around every HTML element. It consists of:<br>
    <strong>margins, borders, padding</strong>, and the actual content.<br>
    <strong>Content</strong> - The content of the box, where text and images appear<br>
    <strong>Padding</strong> - Clears an area around the content. The padding is transparent<br>
    <strong>Border</strong> - A border that goes around the padding and content<br>
    <strong>Margin</strong> - Clears an area outside the border. The margin is transparent
    <table id="selectors">
  <tr>
    <th>Example-code</th>
    <th>Example</th>
  </tr>
  <tr>
    <td><code>#boxmodelstyle{<br>
	background-color: lightgrey;<br>
	width: 300px;<br>
	border: 15px solid green;<br>
	padding: 50px;<br>
	margin: 20px;
  }</code>
  </td>
    <td><div id="boxmodelstyle">This text is the content of the box. We have added a 50px padding, 20px margin and a 15px green border. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</div></td>
  </tr>
</table>
<p><strong>Important</strong>: When you set the <code>width</code> and <code>height</code> properties of an element with CSS, you just set the width and height of the content area. To calculate the full size of an element, you must also add padding, borders and margins.</p>
<div>
<strong>Total element width</strong> = width + left padding + right padding + left border + right border + left margin + right margin<br>
<strong>Total element height</strong> = height + top padding + bottom padding + top border + bottom border + top margin + bottom margin<br>
</div>
    </div>

  </main>
</div>

<div class="example">
  <header id="position-info">
    <strong>Position</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice"><p>
    The <code>position</code> property specifies the type of positioning method used for an element (static, relative, fixed, absolute or sticky).<br>
    Elements are then positioned using the top, bottom, left, and right properties. However, these properties will not work unless the position property is set first. They also work differently depending on the position value.<br>
    <table id="selectors">
  <tr>
    <th>Value</th>
    <th>Explanation</th>
  </tr>
  <tr>
    <td>
    <code>position: static;</code>
  </td>
    <td>HTML elements are positioned static by default.<br>Static positioned elements are not affected by the top, bottom, left, and right properties.<br>
    it is always positioned according to the normal flow of the page
    </td>
  </tr>
  <tr>
  <td>
    <code>position: relative;</code>
  </td>
  <td>Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position.<br> Other content will not be adjusted to fit into any gap left by the element.
    </td>
  </tr>
  <tr>
  <td>
    <code>position: fixed;</code>
  </td>
  <td>It is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled.<br> The top, right, bottom, and left properties are used to position the element.<br>
A fixed element does not leave a gap in the page where it would normally have been located.
    </td>
  </tr>
  <tr>
  <td>
    <code>position: absolute;</code>
  </td>
  <td>It is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).<br>
However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.<br>
Note: A "positioned" element is one whose position is anything except static.
    </td>
  </tr>
   <tr>
  <td>
    <code>position: sticky;</code>
  </td>
  <td>It is positioned based on the user's scroll position.<br>
A sticky element toggles between relative and fixed, depending on the scroll position.<br> It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).
    </td>
  </tr>
  <tr>
  <td>
    <code>z-index</code>
  </td>
  <td>When elements are positioned, they can overlap other elements.<br>
The z-index property specifies the stack order of an element (which element should be placed in front of, or behind, the others).<br>
An element can have a positive or negative stack order.
    </td>
  </tr>
</table>
</div>
    </div>

  </main>
</div>
