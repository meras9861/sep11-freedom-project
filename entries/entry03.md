# Entry 3
2/10/2021

### Sources
I decided to do a bit more tinkering with <b>A-Frame</b> throughout the last couple of months to be even more comfortable with all the formatting and designs this tool has to offer. Not only did I use the actual A-Frame website, but I also wanted to watch quick and simple tutorials on how to use this tool on <b>Youtube</b>. Some videos I watched involved <a href="https://www.youtube.com/watch?v=K_1RdCVuu98">building enviornments</a> and <a href="https://www.youtube.com/watch?v=eTFPMxqod2I">example code</a>. These videos were very helpful with introducing the wide variety of strategies I could use to help build the location I want for my Freedom Project. Since I am doing a project revolving around a 360° image of a galaxy setting, these videos gave me countless ideas on what objects would be best to include in my project. Along with these videos, I used and altered code under the <b>"Guides"</b> section on A-Frame (shown in "Knowledge" section of blog entry). I visited <a href="https://aframe.io/docs/1.2.0/guides/building-a-basic-scene.html">"Building a Basic Scene"</a> to understand how to make a shape such as a cube show up on my screen. I also spent a majority of my tinkering time continuing from where I left off with the guide <a href="https://aframe.io/docs/1.2.0/guides/building-a-360-image-gallery.html">"Building a 360° Image Gallery"</a>. These two guides and as well as the supporting Youtube videos I watched have led me in the right diection when choosing what to include in my overall location of my project, which will help me when getting into the specific placements of each and every aspect of the galaxy location I am putting my mini-game in.

### Engineering Design Process
In my <b>engineering design process</b>, I am currently continuing to work on <b>stage 4</b>, which is to plan the most promising solution. From my previous work along this stage, as well as stages 1-3 (defining the problem, researching the problem, and brainstorming possible solutions), I have gathered a large variety of ideas for my mini-game to help give a game that is entertaining to people of all ages. One promising solution I am considering is to make the game at different levels (easy, medium, and hard) so I can give people the choice to play my game at any level of difficulty they would like to play with. This would also be helpful for the range of ages my users may be at. Another promising solution I thought of was to give different prizes to those who win my mini-game bades off of their age in order to ensure that everyone gets a prize that is age appropriate. To do this, I am planning to ask the user how old they are before they start playing the game to identifiy which prize they will recieve if they win beforehand by using an if, else and else, if statments. An example of this code is shown below:
```javascript
  if (age < 10) {
  prize = coloring book;
  } else {
  prize = magazine;
  }
```
Additionally, I am thinking of including characters in my game that range from a child, to an adult, to an elder. This way, my users will be able to play my mini-game with someone similar to themselves. This can make my users feel more comfortable playing my game and allow them to have a virtual buddy alongside them throughout the game (or not if they the user chooses to not have an avatar). These are only some of the many promising solutions I have for my Freedom Project that I think will really make the issue of not having a single game for multiple different age groups be resolved. Soon, I plan to get more further in my enginnering desgin process and begin <b>stages 5 and 6</b>, which is to create a prototype and testing/evaluating that prototype. I will then get to see all of my ideas up close and decide what I may need to take away or what I may need to add to my project to guarantee a great game for everyone.

### Knowledge
Throughout the last few months, my SEP11 class has taught me how to code my work using <b>variables</b> and <b>loops</b> (for and/or while loops). So, I wanted to use all the information I learned from my class (along with my previous knowledge of conditional statements if needed at any point) to modify some of the example codes I have came across when visiting the A-Frame webiste and practice code from Youtube videos/tutorials on what A-Frame can bring to my project, which gave helped me get ideas on how I would like to style my project and what the overall presentation of my project will look like. The first code I wanted to test out using what I am learning in school is from the guide <a href="https://aframe.io/docs/1.2.0/guides/building-a-basic-scene.html">"Building a Basic Scene"</a> on A-Frame.  

A piece of code from <a href="https://aframe.io/docs/1.2.0/guides/building-a-basic-scene.html#adding-a-background-to-the-scene">"Adding a Background to the Scene"</a>:
```javascript
  <a-scene>
  <a-box color="red" position="0 2 -5" rotation="0 45 45" scale="2 2 2"></a-box>

  <a-sky color="#222"></a-sky>
</a-scene>
```

The code above shows how A-Frame uses ```<a-box>``` and ```<a-sky>``` to create a background that surrounds a majority of the screen when the user wnats to move around or if they want to explore the eniornemnt of the website they are on. I wanted to alter this code a bit to include what I have learned about variables from my SEP11 class, as well making everything look more organized and easier to read, which is shown below:

```javascript
<a-scene> {
  var color1 = "maroon"; 
  var position = "0 5 -10"; 
  var rotation = "0 180 180"; 
  var scale = "4 4 4";
  var a-box = "color1" + "position" + "rotation" + "scale";

  var color2 = "#255, 87, 51";
  var a-sky = "color2"; 
}
</a-scene> 
```

To make the code from A-Frame more simple to read and use, I used ```var``` to sepearte all the different aspects of the background instead of keeping everything in one line togther like it was shown on A-Frame, such as color, postion, ect. All of the different variables were then added together in the final ```var``` to give a similar result to the code from A-Frame. Additionally, I changed the values of each variable to test out a different look for a background. This way, I can see multiple perspectives of the scenery I am trying to create. I learned that using ```var``` not only keeps my code more organized, but it also helps me use those same variables throughout my entire project, which helps if I want to change a specific value of a varable since I am planning to have different backgrounds for each level (easy, medium, and hard). I tried this once more with code from another guide called <a href="https://aframe.io/docs/1.2.0/guides/building-a-360-image-gallery.html">"Building a 360° Image Gallery"</a> on A-Frame. 

A piece of code from <a href="https://aframe.io/docs/1.2.0/guides/building-a-360-image-gallery.html#layout-component-to-lay-out-links">"Using Standard Components"</a>:

```javascript
<a-entity class="link"
  geometry="primitive: plane; height: 1; width: 1"
  material="shader: flat; src: #cubes-thumb"></a-entity>
 ```
 
The code above plays in intricate part in inserting a URL for an image to appear as the object I am coding with (in this case a cube). I used ```var``` again to make this code more easier to comprehend and read, which is shown below:
 
```javascript
<a-entity class="link" {
  var primitive: "plane"; 
  var height: "1"; 
  var width: "1";
  var geometry = "primitive" + "height" + "width";
  
  var shader: "flat"; 
  var src: "#cubes-thumb";
  var material= "shader + "src";
  } 
  </a-entity>
```

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
