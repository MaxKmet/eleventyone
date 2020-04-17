---
layout: layout.liquid
pageTitle: LEARN HTML
---
<h1 class="centered_para">Explore HTML</h1>
<div class="flex-container">
  <div class="resizing"><a href="#attributes-info"><strong>Attributes</strong></a></div>
  <div class="resizing"><a href="#media-info"><strong>Media</strong></a></div>
  <div class="resizing"><a href="#tables-info"><strong>Tables</strong></a></div>  
  <div class="resizing"><a href="#forms-info"><strong>Forms</strong></a></div>
  <div class="resizing"><a href="#apis"><strong>APIs</strong></a></div>
</div>

<div class="example">
  <header>
    <strong>HTML: general</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <strong>HTML</strong> is the standard markup language for creating Web pages.
    <ul>
    <li>HTML elements are represented by tags</li>
    <li>Example: <code>&ltp&gtcontent here&lt/p&gt</code></li>
    <li>Usually there is an opening tag (&ltp&gt) and a closing one &lt/p&gt</li>
    <li>But some tags are represented as one tag (e.g. &ltbr/&gt)</li><br>
    <li>The purpose of a web browser (Chrome, Edge, Firefox, Safari) is to read HTML documents and display them properly.</li><br>
    <li>The <code>&lt!DOCTYPE html&gt</code> declaration represents the document type, and helps browsers to display web pages correctly.It must only appear once, at the top of the page (before any HTML tags)</li>
    </ul>
    </div>

  </main>

<div class="example">
  <header id="attributes-info">
    <strong>Attributes: general</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <ul>
    <li>All HTML elements can have attributes</li>
    <li>Attributes provide additional information about an element</li>
    <li>Attributes are always specified in the start tag</li>
    <li>Attributes usually come in name/value pairs like: name="value"</li>
    </ul>
    </div>

  </main>
</div>

  <header>
    <strong>Attributes</strong>
  </header>
  <main class="main" \>
    <div class="left-content">
      class<br>
      href<br>
      src<br>
      alt<br>
      id<br><br>
      style<br>
      title<br>
      width<br>
    </div>
    <div class="centre-content">
    class of element<br>
    link address<br>
    path/url to source<br>
    text if image failed<br>
    unique id for element<br><br>
    inline style for element<br>
    tooltip<br>
    element width(px,% or other)
    </div>
    <div class="right-content">
    <code>&ltp class="class1&gttext&lt/p&gt</code><br>
    <code>&lta href="some-link"&gt&lt/a&gt</code><br>
     <code>&ltimg src="img.jpg"<br>alt="image&gt</code><br>
     <code>&lta id="link1" href="some-link"&gt&lt/a&gt</code><br>
     <code>&ltp style="color:red"&gtred words&lt/p&gt</code><br>
     <code>&ltp title="tooltip"&gtword&lt/p&gt</code><br>
     <code>&ltp width=50%&gtword&lt/p&gt</code><br>
    </div>
  </main>
  <header>
    <strong id="media-info">Media</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <ul>
    <li>Media examples: Images, music, sound, videos, records and more.</li>
    <li>Web pages often contain multimedia elements of different types and formats.</li><br>
    <li>Video formats supported by the HTML5 standard:</li>
    <li>MP4, WebM, and Ogg</li><br>
    <li>Audio formats supported by the HTML5 standard:</li>
    <li>MP3, WAV, and Ogg </li><br>
    <li>Image formats supported by the HTML5 standard:</li>
    <li>All common</li>
    </ul>
    </div>

  </main>

  <header>
    <strong id="media-info">Images</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    In HTML, images are defined with the &ltimg&gt tag.<br>
    The &ltimg&gt tag is empty, it contains attributes only, and does not have a closing tag.<br>
    The src attribute specifies the URL (web address) of the image:<br>
    <code>&ltimg src="url"&gt</code><br>
    <code>&ltimg src="img_name.jpg" alt="some image" style="width:500px;height:600px;"&gt</code><br>
    The value of the alt attribute should describe the image in case it can't be displayed.<br>
    Use the CSS width and height properties to define the size of the image(preferred) or width and height attributes.<br>
    Example:<br>
    <code>&ltimg src = "/images/death_star_only.png" width = 100px% height=100px&gt</code><br>
    <img src = "/images/death_star_only.png" width = 100px% height=100px><br>
    Image maps:<br>
    The &ltmap&gt tag defines an image-map. An image-map is an image with clickable areas.<br>
    <code>
     &ltimg src="/images/deathstar.jpg" alt="Workplace" usemap="#workmap"&gt
  &ltmap name="workmap"&gt
    &ltarea shape="rect" coords="34,44,270,350" alt="Computer" href="#"&gt
    &ltarea shape="rect" coords="290,172,333,250" alt="Phone" href="#"&gt
    &ltarea shape="circle" coords="337,300,44" alt="Coffee" href="#"&gt
  &lt/map&gt 
    </code><br>
    Now use following syntax to apply the map to image:
    <br><code>
    &ltimg src="/images/deathstar.jpg" alt="dstar" usemap="#workmap"&gt
    </code><br>
    Alternative text example:
     <img src="workplace.jpg" alt="Workplace" usemap="#workmap">
<br>Working example:
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="#">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="#">
  <area shape="circle" coords="337,300,44" alt="Coffee" href="#">
</map> 
    <img src="/images/deathstar.jpg" alt="dstar" usemap="#workmap" width=500em height=250em>
    <br><br>
    Background images:<br>
    Use the style attribute to define background image<br>
    <code>
    &ltdiv style="background-image: url('/images/stardestroyer.jpg')"&gt&ltbr&gt&ltbr&gt&ltbr&gt&lt/div&gt
    </code>
    <div style="background-image: url('/images/stardestroyer.jpg')"><br><br><br></div>
    <br>
    To avoid the background image from repeating itself, use the background-repeat property.<br>
    To make sure the entire element is always covered, set the background-attachment property to fixed<br>
    <code>background-repeat: no-repeat;<br>background-attachment: fixed;<br>
  background-size: cover;</code>
  </div></main>
  <header>
    <strong>Videos</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <ul>
    <li>Before HTML5, a video could only be played in a browser with a plug-in (like flash).</li>
    <li>The HTML5 &ltvideo&gt element specifies a standard way to embed a video in a web page.</li><br>
    <li>The controls attribute adds video controls, like play, pause, and volume.</li>
<li>It is a good idea to always include width and height attributes. If height and width are not set, the page might flicker while the video loads.<li>
<li>The &ltsource&gt element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.</li>
<li>The text between the opening and closing tags will only be displayed in browsers that do not support the &ltvideo&gt element.</li>
    <br>
    Example code:<br>
    <code>
     &ltvideo width="320" height="240" autoplay&gt
  &ltsource src="movie.mp4" type="video/mp4"&gt
  &ltsource src="movie.ogg" type="video/ogg"&gt
Your browser does not support the video tag.
&ltvideo&gt<br>
</code>
    </ul>
    </div>
  </main>


  <header>
    <strong>Audio</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <ul>
    <li>Before HTML5, a audio could only be played in a browser with a plug-in (like flash).</li>
    <li>The HTML5 &ltaudieo&gt element specifies a standard way to embed audio in a web page.</li><br>
    <li>The controls attribute adds video controls, like play, pause, and volume.</li>
    <br>
    Example:<br>
    <code>
      &ltaudio controls&gt
  &ltsource src="/images/trump.mp3" type="audio/mpeg"&gt
Your browser does not support the audio element.
&lt/audio&gt <br>
<audio controls>
  <source src="/images/trump.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
</code>
    </ul>
    </div>
  </main>
    <header id="tables-info">
    <strong>Tables</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <ul>
    <li>Use the HTML &lttable&gt element to define a table</li>
    <li>Use the HTML &lttr&gt element to define a table row</li>
    <li>Use the HTML &lttd&gt element to define a table data</li>
    <li>Use the HTML &ltth&gt element to define a table heading</li>
    <li>Use the HTML &ltcaption&gt element to define a table caption</li>
    <li>Use the colspan attribute to make a cell span many columns</li>
    <li>Use the rowspan attribute to make a cell span many rows</li>
    <br>
    Basic code example can be found on <a href="/tutorials/html_jedi">LEARN HTML</a> page
    </ul>
    </div>
  </main>

   <header id="forms-info">
    <strong>Forms</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <ul>
    <li>The HTML &ltform&gt element defines a form that is used to collect user input</li>
    <li>The &ltinput&gt element is the most important form element.</li>
    <li>The &ltinput&gt element is displayed in several ways, depending on the type attribute.</li><br>
    <li><strong>Type attributes:</strong></li>
    <li><code>type="text"</code> - Defines a single-line text input field</li>
    <li><code>type="radio"</code> - Defines a radio button (for selecting one of many choices)</li>
    <li><code>type="submit"</code> - Defines a submit button (for submitting the form)</li>
    <li><code>type="password"</code> - defines a password field</li>
    <li><code>type="reset"</code> - defines a reset button that will reset all form values to their default values</li>
    <li><code>type="checkbox"</code> - defines a checkbox</li>
    <li><code>type="button"</code> - defines a button</li>
    <li><code>type="color"</code> - used for input fields that should contain a color</li>
    <li><code>type="date"</code> is used for input fields that should contain a date</li>
    <li><code>type="email"</code> is used for input fields that should contain an e-mail address</li>
    <li><code>type="file"</code> defines a file-select field and a "Browse" button for file uploads</li><br>
    <li><strong>Input attributes:</strong></li>
    <li><code>value</code> - attribute specifies an initial value for an input field</li>
    <li><code>readonly</code> - attribute specifies that an input field is read-only</li>   
    <li><code>disabled</code> - attribute specifies that an input field should be unusable and un-clickable</li>
    <li><code>size</code> - attribute specifies the visible width, in characters, of an input field.</li>
    <li><code>placeholder</code> - attribute specifies short a hint that describes the expected value of an input field</li>
    <li><code>required</code> - attribute specifies that an input field must be filled out before submitting the form</li>
    <li></li>
    </ul><br>
    Example:<br>
    <code>
    &ltform>
  &ltlabel for="favcolor">Select your favorite color:&lt/label&gt
  &ltinput type="color" id="favcolor" name="favcolor"&gt
&lt/form&gt
    </code>
    
  <form>
  <label for="favcolor">Select your favorite color:</label>
  <input type="color" id="favcolor" name="favcolor">
  </form> <br>
    More code example can be found on <a href="/tutorials/html_jedi">LEARN HTML</a> page
    </div>
  </main>


  <header id="apis">
    <strong>HTML5 APIs</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    <ul>
    <li><strong>HTML5</strong> provides various APIs like:</li>
    <li>Geolocation</li>
    <li>Web storage</li>
    <li>Drag/Drop</li>
    <li>Web Workers</li><br>
    <li>But working with them requires understanding of JS</li>
    </ul>
    </div>
  </main>

  <header>
    <strong>Next steps</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    Next we suggest you learn <strong>CSS</strong>.<br>
    Press the spaceship to fly to CSS page.
    <a href="/tutorials/css_jedi">
                        <img class="sword" src = "/images/death_star_only.png" width = 50%>
    </a>
    </div>
  </main>
  </div>
</main>













