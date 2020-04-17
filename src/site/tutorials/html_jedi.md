---
layout: layout.liquid
pageTitle: LEARN HTML
---

<div class="example">
  <header>
    <strong>Basic HTML tags</strong>
  </header>
  <main class="main">
    <div class="left-content">
      &lthtml&gt<br>
      &lthead&gt<br>
      &ltbody&gt<br>
      &lttitle&gt<br>
      &ltp&gt<br>
      &ltdiv&gt<br>
      &ltbr/&gt<br><br>
      &lti&gt<br>
      &ltdel&gt<br>
      &lth1-6&gt<br>
      &lthr/&gt<br>
      &lta href="#"&gt&lt/a&gt<br><br>
      &ltol&gt/&ltul&gt+&ltli&gt<br>ol-ordered list<br>ul-unordered list<br>li-list element
    </div>
    <div class="centre-content">
      start and end of document<br>
      meta data<br>
      visual content<br>
      browser title + SEO<br>
      paragraph of text<br>
      block of content<br>
      line<br>break<br>
      <i>italic</i><br>    
      <del>crossed</del><br>
      <h3>headline3</h3>
      <hr/>
      <a href="#">link</a><br><br>
    <ol>
        <li>1.Ordered</li>
        <li>2.list</li>
        <li>3.elements</li>
    </ol>  
    </div>
    <div class="right-content">
    &lthtml&gt...&lt/html&gt<br>
    &lthead&gt...&lt/head&gt<br>
    &ltbody&gt...&lt/body&gt<br>
    &lttitle&gt...&lt/title&gt<br>
    &ltp&gtparagraph&lt/p&gt<br>
    &ltdiv&gtcontent&lt/div&gt<br>
    line&ltbr/&gtbreak<br><br>
    &lti&gtitalic&lt/i&gt<br>
    &ltdel&gtcrossed&lt/del&gt<br>
    &lth3&gtheadline3&lt/h3&gt<br>
    &lthr/&gt<br>
    &lta href="#"&gt&lt/a&gt<br><br>
    &ltol&gt<br>
        &ltli&gtOrdered&lt/li&gt<br>
        &ltli&gtlist&lt/li&gt<br>
        &ltli&gtelements&lt/li&gt<br>
    &lt/ol&gt<br>
    </div>
  </main>

  <header>
  <strong>
    Table example
  </strong>
  </header>
  <main class="main">
    <div class="left-content">
      &lttable&gt<br>
      &lttr&gt-table row<br>
      &lttd&gt-table data<br>
      colspan-number of columns to span<br>
    </div>
    <div class="centre-content">
      <table border="2">
        <tr>
      <td>One</td>
      <td>Two</td>
      <td>Three</td>
        </tr>
        <tr>
      <td><br /></td>
      <td colspan="2"><br /></td>
        </tr>
        </table>
    </div>
    <div class="right-content">
      &lttable border="2"><br>
        &lttr&gt<br>
      &lttd&gtOne&lt/td&gt<br>
      &lttd&gtTwo&lt/td&gt<br>
      &lttd&gtThree&lt/td&gt<br>
        &lt/tr&gt
        &lttr&gt<br>
      &lttd&gt<br />&lt/td&gt<br>
      &lttd colspan="2"&gt<br />&lt/td&gt<br>
        &lt/tr&gt<br>
        &lt/table&gt<br>
    </div>
  </main>

  <header>
  <strong>
    Forms
  </strong>
  </header>
  <main class="main">
    <div class="left-content">
      &ltform&gt<br>
      action<br>
      method<br><br><br><br><br><br><br>
      input type<br>
    </div>
    <div class="centre-content">
    Collect data from user<br>
    Link to load after submit<br>
    HTTP method (POST/GET) to use when submit<br>
    POST - offers better security(data is not visible in the page address)<br>
    GET - data is visible in the page address<br>
    text<form><input type="text" name="username" /></form>
    password<form><input type="password" name="username" /></form>
    radio<br><form><input type="radio" name="username" /></form>
    checkbox<br><form><input type="checkbox" name="username" /></form>
    submit<br><form><input type="submit" value="press" /></form>
    Tip: "name" attribute is used to get value from js code
    </div>
    <div class="right-content">
    &ltform action="#link" method="POST"&gt 
    &lt/form&gt<br><br><br><br><br><br><br>
    <small>&ltform&gt&ltinput type="text" name="username"/&gt&lt/form&gt</small><br>
    <small>&ltform&gt&ltinput type="password" name="username"/&gt&lt/form&gt</small><br>
    <small>&ltform&gt&ltinput type="radio" name="username"/&gt&lt/form&gt</small><br>
    <small>&ltform&gt&ltinput type="checkbox" name="username"/&gt&lt/form&gt</small><br>
    <small>&ltform&gt&ltinput type="submit" value="press"/&gt&lt/form&gt</small><br>
    </div>
  </main>
  <main class="main">
    <div class="left-content">
    <strong><u>Not enough ?</u></strong>
    Press the spaceship if you wanna deeper understanding of <i>HTML</i>
    </div>
    <div class="centre-content">
    <a href="/tutorials/html_more">
                        <img class="sword" src = "/images/death_star_only.png" width = 90%>
                        </a>
    </div>
    <div class="right-content">
    </div>
  </main>
  
</div>




