### 🧠 html brain activity

## <sub>table of contents</sub>
- [forms](#forms)
- [links](#links)
- [lists](#lists)
- [media](#media)
- [tables](#tables)
- [text](#text)

## <sub>forms</sub>
|<sub>properties</sub>|<sub>action</sub>|
| :-: | :- |
|<sub>form</sub>|<sub>printed document that contains spaces for user to fill in information</sub>|
|<sub>methods</sub>|<sub>- **get**: values are added to the end of the URL specified in the action attribute (use if form is short or is just retrieving data from the web server).<br/>- **post**: values sent in HTTP headers (use if form allows user to upload a file, is very long and contains sensitive data, or adds/deletes information from a database)<br/>|
|<sub>type</sub>|<sub>- **text**: input values can only be text and are on a single line<br/>- **password**: input values are masked, but act like a text type<br/>- **radio**: buttons for user to select from only 1<br/>- **checkbox**: buttons for user to select as many as they want<br/>- **file**: input and button to browse computer for a file<br/>- **submit**: button to send form to server<br/>- **image**: adds an image to the button (acts like an image element)<br/>- **hidden**: value hidden from the page<br/>- **date**: value is in the format of a date<br/>- **email**: value is checked if it is a valid email<br/>- **url**: value is checked if it is a valid url<br/>- **search**: input for search queries<br/></sub>|
 
### <sub>text fields/inputs</sub>
```html
<!-- container for the form controls. action contains the link that will receive form information -->
<form action=“http://link” method=“get"> 
  <input 
    <!-- specifies the type of input -->
    type=“text”
    <!-- identification of form control to be sent to the server -->
    name=“username” 
    <!-- limits the number of characters allowed -->
    maxLength=“10”
    <!-- form validation -->
    required=“required” 
    <!-- text to indicate what the form control is used for -->
    placeholder=“username”
  /> 
  <button>Hello</button> 
</form>
```

### <sub>radio buttons/checkboxes</sub>
```html
<form action=“http://link” method=“get>                                                     
  <input 
    <!-- change to checkbox if you want multi-select -->
    type=“radio” 
    name=“genre” 
    <!-- indicates the value that is sent to the server for the selected option -->
    value=“rock”
    <!-- selected value on page load -->
    checked=“checked” 
  /> 
  <input 
    type=“radio” 
    name=“genre” 
    value=“pop”
  />
  <input 
    type=“radio” 
    name=“genre” 
    value=“country” 
  />
</form>
```

### <sub>dropdowns</sub>
```html
<form action=“http://link">
  <select -> used to create the dropdown
    name="cars” 
    id=“cars”
    <!-- number of options shown at once -->
    size=“3”
    <!-- allows user to select multiple options -->
    multiple=“multiple"
  >
    <!-- used to create an element in the dropdown -->
    <option value="volvo">Volvo</option> 
    <!-- selected value on page load -->
    <option value=“saab” selected=“selected">Saab</option> 
    <option value="opel">Opel</option>
    <option value="audi">Audi</option>
  </select>
</form>
```

### <sub>grouping</sub>
```html
<!-- grouping of form controls -->
<fieldset> -> grouping of form controls
  <!-- text to label a group of form controls -->
  <legend>Login</legend> 
  <!-- text to label the form control -->
  <label>Username:</label>
  <input 
    type=“text” 
    name=“username”
    maxLength=“10” 
  /> 
  <label>Password:</label>
  <input 
    type=“password” 
    name=“password”
    maxLength=“10”
  /> 
</fieldset> 
```

## <sub>links</sub>
```html
<!-- link -->   
<a href=“http://link”>Link</a> 

<!-- email link -->        
<a href=“mailto:test@test.com”>Email</a>  

<!-- open new window link -->        
<a href=“http://link” target=“_blank">Link</a>

<!-- same page with id bottom link -->                                    
<a href=“#bottom”>Link</a>
                                     
<!-- another page with id bottom link -->   
<a href=“http://url/#bottom”>Link</a>
```

## <sub>lists</sub>
##### ordered/numbered
```html
<ol>
  <li>Apple</li> 
  <li>Banana</li> 
  <li>Orange</li>
  <li>Kiwi</li>
</ol> 
```
##### unordered/bullet
```html
<ul>
  <li>Apple</li> 
  <li>Banana</li> 
  <li>Orange</li>
  <li>Kiwi</li>
</ul> 
```
##### definition
```html
<dl>
  <dt>Fruit:</dt>
  <dd>Apple</dd> 
  <dd>Banana</dd> 
  <dd>Orange</dd>
  <dd>Kiwi</dd>
</dl> 
```

## <sub>media</sub>
### <sub>images</sub>
|<sub>term</sub>|<sub>definition</sub>|
| :-: | - |
|<sub>svg</sub>|<sub>scalable vector graphics <br/> type of image format</sub>|
```html
<img 
  src=“images/img.png” 
  alt=“image description” 
  title=“description (tooltip)” 
  height=“600” <!-- defaulted to pixels --> 
  width=“600”  <!-- defaulted to pixels --> 
  align="left" <!-- allows the picture to be displayed next to body of text, not integrated into text --> 
/>  
```

### <sub>audio</sub>
|<sub>properties</sub>|<sub>action</sub>|
| :-: | :- |
|<sub>controls</sub>|<sub>indicates whether or not the player should display controls</sub>|
|<sub>autoplay</sub>|<sub>indicates that the audio should start playing automatically</sub>|
```html
<audio controls autoplay>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  <p>Your browser does not support the audio element.</p>
</audio>
```

### <sub>video</sub>
|<sub>properties</sub>|<sub>action</sub>|
| :-: | :- |
|<sub>preload</sub>|<sub>tells the browser what to do when the page loads<br/>- **none**: browser shouldn’t load the video until the user presses play<br/>- **auto**: browser should download the video when the page loads<br/>- **metadata**: browser should just collect information (_**EX: size, 1st frame, track list, duration**_)</sub>|
|<sub>poster</sub>|<sub>specify an image to show while the video is downloading or until the user plays the video</sub>|
|<sub>width</sub>|<sub>specifies the width of the frame</sub>|
|<sub>height</sub>|<sub>specifies the height of the frame</sub>|
|<sub>controls</sub>|<sub>indicates that the browser should supply its own controls for playback</sub>|
|<sub>autoplay</sub>|<sub>indicates that the video should start playing automatically</sub>|
|<sub>loop</sub>|<sub>indicates that the video should start playing again once it has ended<br/>browser should supply its own controls for playback<br/>date must be specified</sub>|
```html
<video width="400" controls>
  <source src="mov_bbb.mp4" type="video/mp4">
  <source src="mov_bbb.ogg" type="video/ogg">
  <p>Your browser does not support the audio element.</p>
</video>  
```

## <sub>tables</sub>
|<sub>property</sub>|<sub>action</sub>|
| :-: | :- |
|<sub>table</sub>|<sub>representation of information in a grid format (_**EX: TV Schedules, Financial Reports, etc.**_)</sub>|

```html
<!-- container for the table -->
<table> 
  <!-- headings of the table -->
  <thead>
    <!-- container for the elements in a row -->
    <tr> 
      <!-- header items in a table to either a column or row -->
      <th></th>
      <th scope=“col”>Fruit</th>
      <th scope=“col”>Veggies</th>
    </tr>
  </thead>
  <!-- body of the table -->
  <tbody> 
    <tr>
      <th scope=“row”>Orange Color</th>
      <!-- items in the table -->
      <td>Orange</td> 
      <td>Carrot</td>
    </tr>
    <tr>
      <th scope=“row”>Red Color</th>
      <td>Apple</td>
      <td>Beet</td>
    </tr>
    <tr>
      <th scope=“row”>Green Color</th>
      <td>Kiwi</td>
      <td>Lettuce</td>
    </tr>
  </tbody>
  <!-- footer of the table -->
  <tfoot> 
    <tr>
      <td></td>
      <td colspan="2">Fruit and Veggies are great!</td>
    </tr>
  </tfoot>
</table>
```

## <sub>text</sub>
### <sub>headers</sub>
```html
<h1></h1> 
<h2></h2>                                                            
<h3></h3> 
<h4></h4>
<h5></h5>
<h6></h6> 
```
### <sub>bold</sub>
```html
<b></b>
<!-- indicates significant importance -->
<strong></strong>  
```
### <sub>italic</sub>
```html
<i></i>
<!-- indicates emphasis that subtly changes the meaning of a sentence -->
<em></em>
<!-- cites a piece of work -->
<cite></cite>      
<!-- indicates a defining instance of a new term -->
<dfn></dfn>
```
### <sub>underline</sub>
```html
<ins></ins> 
```
### <sub>strikethrough</sub>
```html
<!-- indicates something is no longer accurate or relevant -->
<s></s> 
<!-- shows content that has been deleted from the document  -->
<del></del>
```
### <sub>superscript/subscript</sub>
```html
<sup></sup> 
<sub></sub>
```
### <sub>break</sub>
```html
<!-- line break, starts the text after it on a new line -->
<br/> 
<!-- creates a horizontal line between elements  -->
<hr/> 
```
### <sub>quotes/abbreviations</sub>
```html
<!-- block quote indentation for longer quotes -->
<blockquote></blockquote>
<!-- adds quotes to text and is used for shorter quotes -->
<q></q>
<!-- indicates an abbreviation -->
<abbr title=“full name”>abbreviation</abbr> 
```
### <sub>contact</sub>
```html
<!-- holds the contact details for the author of the page -->
<address></address>                                
```

