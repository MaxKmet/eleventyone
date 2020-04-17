---
layout: layout.liquid
pageTitle: LEARN HTML
---
<h1 class="centered_para">Explore CSS</h1>
<div class="flex-container">
  <div class="resizing"><a href="#flexinfo"><strong>Flexbox</strong></a></div>
  <div class="resizing"><a href="#dropdowns-info"><strong>Dropdown</strong></a></div>
  <div class="resizing"><a href="#animationinfo"><strong>Animation</strong></a></div>  
</div>


<div class="example">
  <header id="flexinfo">
    <strong>Flexbox</strong>
  </header>
  <main class="main">
    <div class="right-content" class="basic_artice">
    The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.<br>
    The flex container becomes flexible by setting the display property to flex. Here are a few examples:
<table id="selectors">
  <tr>
    <th>HTML</th>
    <th>CSS</th>
    <th>RESULT</th>
  </tr>
  <tr>
    <td>
    <code>
    &ltdiv class="flex-container1"><br>
  &ltdiv&gt1&lt/div&gt<br>
  &ltdiv&gt2&lt/div&gt<br>
  &ltdiv&gt3&lt/div&gt<br>
&lt/div&gt
</code>
</td>
    <td><code>.flex-container1 {<br>
	display: flex;<br>
	background-color: DodgerBlue;<br>
  }<br>
  .flex-container1 > div {<br>
	background-color: #f1f1f1;<br>
	margin: 10px;<br>
	padding: 20px;<br>
	font-size: 30px;
  }</code></td>
    <td><div class="flex-container1">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div></td>
  </tr>
  <tr>
    <td><code>
    &ltdiv class="flex-container2"><br>
  &ltdiv&gt1&lt/div&gt<br>
  &ltdiv&gt2&lt/div&gt<br>
  &ltdiv&gt3&lt/div&gt<br>
&lt/div&gt
</code></td>
    <td><code>.flex-container2 {
	display: flex;
	flex-direction: column;
	background-color: DodgerBlue;
  }
  .flex-container2 > div {<br>
	background-color: #f1f1f1;<br>
	width: 100px;<br>
	margin: 10px;<br>
	text-align: center;<br>
	line-height: 75px;<br>
	font-size: 30px;
  }</code></td>
    <td>
    <div class="flex-container2">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
    </div>
    </td>
  </tr>
  <tr><
    <td colspan=3>
    The <code>"align-items: center;"</code> aligns the flex items in the middle of the container:
    </td>
  </tr>
  <tr>
    <th>HTML</th>
    <th colspan=2>CSS</th>
  </tr>
  <tr>
    <td colspan=1>
    <code>
    &ltdiv class="flex-container3"><br>
  &ltdiv&gt1&lt/div&gt<br>
  &ltdiv&gt2&lt/div&gt<br>
  &ltdiv&gt3&lt/div&gt<br>
&lt/div&gt
</code>
    </td>
    <td colspan=2>
    <code>
      .flex-container3 {<br>
	display: flex;<br>
	justify-content: center;<br>
	background-color: DodgerBlue;<br>
  }<br>
  .flex-container3 > div {<br>
	background-color: #f1f1f1;<br>
	width: 100px;<br>
	margin: 10px;<br>
	text-align: center;<br>
	line-height: 75px;<br>
	font-size: 30px;<br>
  }
  </code>
  </td>
  <tr>
    <td colspan=3>
<div class="flex-container3">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>
</td>
<tr><
    <td colspan=3>
    The <code>"align-items: baseline;"</code> The baseline value aligns the flex items such as their baselines aligns:
    </td>
</tr>
<tr>
    <th>HTML</th>
    <th colspan=2>CSS</th>
</tr>
<tr>
<td colspan=1>
<code>
&lttd&gt<br>
  &ltdiv class="flex-container4"&gt<br>
  &ltdiv&gt&lth1&gt1&lt/h1&gt&lt/div&gt<br>
  &ltdiv&gt&lth6&gt2&lt/h6&gt&lt/div&gt<br>
  &ltdiv&gt&lth3&gt3&lt/h3&gt&lt/div&gt<br>
  &ltdiv&gt&ltsmall&gt4&lt/small>&lt/div&gt<br>  
&lt/div&gt<br>
  &lt/td&gt
  </code>
</td>
<td colspan=2><code>
.flex-container4 {<br>
	display: flex;<br>
	height: 200px;<br>
	align-items: baseline;<br>
	background-color: DodgerBlue;<br>
  }<br>
  .flex-container4 > div {<br>
	background-color: #f1f1f1;<br>
	width: 100px;<br>
	margin: 10px;<br>
	text-align: center;<br>
	line-height: 75px;<br>
	font-size: 30px;<br>
  }</code>
</td>
</tr>
<tr>
  <td colspan=3>
  <div class="flex-container4">
  <div><h1>1</h1></div>
  <div><h6>2</h6></div>
  <div><h3>3</h3></div>  
  <div><small>4</small></div>  
</div>
  </td>
</tr>
</table>
    </div>
  </main>
</div>


<div class="example">
  <header id="dropdowns-info">
    <strong>Dropdown</strong>
  </header>
    <table id="selectors">
  <tr>
    <th>HTML</th>
    <th>CSS</th>
    <th>Example</th>
  </tr>
  <tr>
  
  <td>
    <code>
    &ltdiv class="dropdown"&gt<br>
  &ltbutton class="dropbtn"&gtDropdown&lt/button&gt<br>
  &ltdiv class="dropdown-content"&gt<br>
    &lta href="#"&gtLink 1&lt/a&gt<br>
    &lta href="#"&gtLink 2&lt/a&gt<br>
    &lta href="#"&gtLink 3&lt/a&gt<br>
  &lt/div&gt
    </code>

  </td>
   <td>
   <code>
    .dropbtn {<br>
  background-color: #4CAF50;<br>
  color: white;<br>
  padding: 16px;<br>
  font-size: 16px;<br>
  border: none;<br>
  cursor: pointer;<br>
}<br>
/* The container div - needed to position the dropdown content */<br>
.dropdown {<br>
	position: relative;<br>
	display: inline-block;<br>
  }<br>
  /* Dropdown Content (Hidden by Default) */<br>
  .dropdown-content {<br>
	display: none;<br>
	position: absolute;<br>
	background-color: #f9f9f9;<br>
	min-width: 160px;<br>
	box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);<br>
	z-index: 1;<br>
  }
  /* Links inside the dropdown */<br>
  .dropdown-content a {<br>
	color: black;<br>
	padding: 12px 16px;<br>
	text-decoration: none;<br>
	display: block;<br>
  }
  /* Change color of dropdown links on hover */<br>
  .dropdown-content a:hover {background-color: #f1f1f1}<br>
  /* Show the dropdown menu on hover */<br>
  .dropdown:hover .dropdown-content {<br>
	display: block;<br>
  }
  /* Change the background color of the dropdown button when the dropdown content is shown */<br>
  .dropdown:hover .dropbtn {<br>
	background-color: #3e8e41;<br>
  }

   </code>
  </td>


   <td>
   <div class="dropdown">
  <button class="dropbtn">Dropdown</button>
  <div class="dropdown-content">
    <a href="#">Link 1</a>
    <a href="#">Link 2</a>
    <a href="#">Link 3</a>
  </div>
  </td>

  </tr>
 
<tr>
    <th>HTML</th>
<th>CSS</th>
<th id="animationinfo">Animation</th>
</tr>

<tr>
<td>
<code>
&ltdiv id="increasing_animation"&gt&lt/div&gt
</code>
</td>

<td>
<code>
#increasing_animation{<br>
		height: 20em;<br>
		width:20em;<br>
		background-image: url(../images/death_star_only.png);<br>
		background-position: center;<br>
		background-size: cover;<br>
		transition:transform 2s;<br>
	}
<br>
	#increasing_animation:hover{<br>
		transform: scale(1.3); <br>
	}
</code>
</td>

<td><div id="increasing_animation"></div></td>

</tr>

</table>
    </div>
  </main>
</div>


