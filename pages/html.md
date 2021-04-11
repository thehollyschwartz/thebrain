### 🧠 html brain activity

## <sub>table of contents</sub>
- [links](#links)
- [lists](#lists)
- [media](#media)
- [tables](#tables)
- [text](#text)

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
#### images
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
|<sub>term</sub>|<sub>definition</sub>|
| :-: | - |
|<sub>svg</sub>|<sub>scalable vector graphics <br/> type of image format</sub>|

#### audio
```html
<audio controls autoplay>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  <p>Your browser does not support the audio element.</p>
</audio>
```
|<sub>properties</sub>|<sub>action</sub>|
| :-: | :- |
|<sub>controls</sub>|<sub>indicates whether or not the player should display controls</sub>|
|<sub>autoplay</sub>|<sub>indicates that the audio should start playing automatically</sub>|

#### video
```html
<video width="400" controls>
  <source src="mov_bbb.mp4" type="video/mp4">
  <source src="mov_bbb.ogg" type="video/ogg">
  <p>Your browser does not support the audio element.</p>
</video>  
```
|<sub>properties</sub>|<sub>action</sub>|
| :-: | :- |
|<sub>preload</sub>|<sub>tells the browser what to do when the page loads<br/>- **none**: browser shouldn’t load the video until the user presses play<br/>- **auto**: browser should download the video when the page loads<br/>- **metadata**: browser should just collect information (_**EX: size, 1st frame, track list, duration**_)</sub>|
|<sub>poster</sub>|<sub>specify an image to show while the video is downloading or until the user plays the video</sub>|
|<sub>width</sub>|<sub>specifies the width of the frame</sub>|
|<sub>height</sub>|<sub>specifies the height of the frame</sub>|
|<sub>controls</sub>|<sub>indicates that the browser should supply its own controls for playback</sub>|
|<sub>autoplay</sub>|<sub>indicates that the video should start playing automatically</sub>|
|<sub>loop</sub>|<sub>indicates that the video should start playing again once it has ended<br/>browser should supply its own controls for playback<br/>date must be specified</sub>|

## <sub>tables</sub>
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
|<sub>term</sub>|<sub>definition</sub>|
| :-: | :- |
|<sub>table</sub>|<sub>representation of information in a grid format (_**EX: TV Schedules, Financial Reports, etc.**_)</sub>|

## <sub>text</sub>
### <sub> headers</sub>
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

