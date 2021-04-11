### 🧠 html brain activity

## <sub>table of contents</sub>
- [media](#media)
- [links](#links)
- [lists](#lists)

#### benefits
<ol>
  <sub><li>**Cross Browser Compatibility** - Most browsers support websites built with HTML, which means that the user can use their preferred browser (hopefully is chrome 😜) when viewing a website.</li></sub>
  <li>hello</li>
</ol>
<sub>**Cross Browser Compatibility** - Most browsers support websites built with HTML, which means that the user can use their preferred browser (hopefully is chrome 😜) when viewing a website.</sub>

- Doctype.
  - Simple and short.
- Improved Accessibility.
- Cleaner Code.
- Mobile Optimization.
- Cross Browser Compatible.
- Audio/Video Support.
  - Using the <audio> and <video> tags.
- Geolocation.
  - Detect user location to relate to them.
- Intriguing Interface.
  - Drawing element allows animation and more.
- Game Development.
  - Using the <canvas> tag.
- Improved Storage.



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
```
<ol>
  <li>Apple</li> 
  <li>Banana</li> 
  <li>Orange</li>
  <li>Kiwi</li>
</ol> 
```
##### unordered/bullet
```
<ul>
  <li>Apple</li> 
  <li>Banana</li> 
  <li>Orange</li>
  <li>Kiwi</li>
</ul> 
```
##### definition
```
<dl>
  <dt>Fruit:</dt>
  <dd>Apple</dd> 
  <dd>Banana</dd> 
  <dd>Orange</dd>
  <dd>Kiwi</dd>
</dl> 
```
