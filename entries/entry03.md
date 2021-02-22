# Entry 3
2/10/2021

### Sources
I decided to do a bit more tinkering with <b>A-Frame</b> throughout the last couple of months to be even more comfortable with all the formatting and designs this tool has to offer. Not only did I use the actual A-Frame website, but I also wanted to watch quick and simple tutorials on how to use this tool on <b>Youtube</b>. Some videos I watched involved <a href="https://www.youtube.com/watch?v=K_1RdCVuu98">building enviornments</a> and <a href="https://www.youtube.com/watch?v=eTFPMxqod2I">example code</a>. These videos were very helpful in introducing the wide variety of strategies I could use to help build the location I want for my Freedom Project. Since I am doing a project revolving around a 360° image of a galaxy setting, these videos gave me countless ideas on what objects would be best to include in my project. 

Along with these videos, I used and altered code under the <b>"Guides"</b> section on A-Frame (code is shown in the "Knowledge" section of this blog entry). I visited <a href="https://aframe.io/docs/1.2.0/guides/building-a-basic-scene.html">"Building a Basic Scene"</a> to understand how to make a shape such as a cube show up on my screen. I also spent a majority of my tinkering time continuing from where I left off with the guide <a href="https://aframe.io/docs/1.2.0/guides/building-a-360-image-gallery.html">"Building a 360° Image Gallery"</a>. These two guides and the supporting Youtube videos I watched have led me in the right direction when choosing what to include in the final location of my project, which will help me when getting into the specific placements of each and every aspect of the galaxy location I am putting in my mini-game.

### Engineering Design Process
In my <b>engineering design process</b>, I am currently continuing to work on <b>stage 4</b>, which is to plan the most promising solution. From my previous work along this stage, as well as stages 1-3 (defining the problem, researching the problem, and brainstorming possible solutions), I have gathered a large variety of ideas for my mini-game to help me make a game that is entertaining to people of all ages. One promising solution I am considering is to make the game at different levels (easy, medium, and hard) so I can give my users the choice to play my game at any level of difficulty they would like. This would also be helpful for the range of ages my users may be at. Another promising solution I thought of was to give different prizes to those who win my mini-game based on their age to ensure that everyone gets an age-appropriate prize. To do this, I am planning to ask the user certain questions like how old they are before they start playing my game to identify which prize they will receive if they win beforehand by using an if, else, or else, if statement. An example of this code is shown below:

```javascript
  if (age < 10) {
  prize = coloring book;
  } else {
  prize = magazine;
  }
```

Additionally, I am thinking of including characters in my game that range from a child, to an adult, to an elder. This way, my users will be able to play my mini-game with someone similar to themselves. This can make my users feel more comfortable playing my game and allow them to have a virtual buddy alongside them throughout the game (or not if the user chooses to not have an avatar). These are only some of the many promising solutions I have for my Freedom Project that I believe will make the issue of not having a single game for different age groups be resolved. 

Soon, I plan to get more further in my engineering design process and begin <b>stages 5 and 6</b>, which is to create a prototype and testing/evaluating that prototype. I will then get to see all of my ideas up close and decide what I may need to take away, or what I may need to add to my project to guarantee a great game for everyone.

### Knowledge
Throughout the last few months, my SEP11 class has taught me how to code my work using <b>variables</b> and <b>conditional statements</b>. So, I wanted to use all the information I learned from my class to modify some of the example codes I have come across when visiting the A-Frame website, which helped me get ideas on how I would like to style my project and what the overall presentation of my project will look like. The first code I wanted to test out using what I am learning in school is from the guide <a href="https://aframe.io/docs/1.2.0/guides/building-a-basic-scene.html">"Building a Basic Scene"</a> on A-Frame.  

A piece of code from <a href="https://aframe.io/docs/1.2.0/guides/building-a-basic-scene.html#adding-a-background-to-the-scene">"Adding a Background to the Scene"</a>:

```javascript
  <a-scene>
  <a-box color="red" position="0 2 -5" rotation="0 45 45" scale="2 2 2"></a-box>

  <a-sky color="#222"></a-sky>
</a-scene>
```

The code above shows how A-Frame uses ```<a-box>``` and ```<a-sky>``` to create a background that surrounds a majority of the screen when the user wants to move around, or if the user wants to explore the environment of the website they are on. I wanted to alter this code a bit to include what I have learned about variables from my SEP11 class, as well making everything look more organized and easier to read, which is shown below:

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

To make the code from A-Frame more simple to read and use, I used ```var``` to separate all the different aspects of the background instead of keeping everything in one line together like it was shown on A-Frame, such as color, position, etc. All of the different variables were then added together in the final ```var``` to give a similar result to the code from A-Frame. Additionally, I changed the values of each variable to test out a different look for the background. This way, I can see multiple perspectives of the scenery I am trying to create. I learned that using ```var``` not only keeps my code more organized, but it also helps me use those same variables throughout my entire project, which helps me if I want to change a specific value of a variable since I am planning to have different backgrounds for each level (easy, medium, and hard) in my mini-game. I tried this once more with code from another guide called <a href="https://aframe.io/docs/1.2.0/guides/building-a-360-image-gallery.html">"Building a 360° Image Gallery"</a> on A-Frame. 

A piece of code from <a href="https://aframe.io/docs/1.2.0/guides/building-a-360-image-gallery.html#layout-component-to-lay-out-links">"Using Standard Components"</a>:

```javascript
<a-entity class="link"
  geometry="primitive: plane; height: 1; width: 1"
  material="shader: flat; src: #cubes-thumb"></a-entity>
 ```
 
The code above plays an intricate part in inserting a URL for an image to appear on the object I am coding with (in this case a cube). I used ```var``` again to make this code more easier to comprehend and read, as well as changing some of the values of each variable to experiment with different looks for the cube, which is shown below:
 
```javascript
<a-entity class = "link" {
  var primitive = "plane"; 
  var height = "5"; 
  var width = "5";
  var geometry = "primitive" + "height" + "width";
  
  var shader = "elevated"; 
  var src = "#cubes-thumb";
  var material = "shader" + "src">;
} 
  </a-entity>
```

Another idea I had to interpret what I am learning in class is using <b>conditional statements</b> (if, else, and else, if statements) to collect user input. An example of what this code would look like is shown below:

```javascript
{
  if(answer == "correct"){
  score++;
  } else if(answer == "incorrect"){
  score--;
  }
}
```

The code above will help my users win my mini-game. If they choose the correct answer, they will get a point added to their score (and a point taken away from their score if they choose the incorrect answer) up until they reach the certain amount of points they chose to play up to. 

These are some of the ideas/alterations I have made using the strategies I have learned from class about variables and conditional statements. 

### Skills
I have gained several <b>skills</b> from my previous blog entry and throughout the last few months. The first <b>skill</b> that I have gained even more from my previous entry is <b>attention to detail</b>, which includes spelling things correctly, adhering to syntax rules, etc. This would have to be the most dominant skill I gained during the last few months because I was using and modifying so many different pieces of code while I was continuing to tinker with/learn my tool. Paying attention to every detail in my code is extremely important because something as small as a curly bracket can throw my entire code off. So, using this skill helped me alter each of the pieces of code I found an interest in because it allowed me to see what mistakes I needed to fix for it to function correctly, as well as learning how each syntax rule plays an intricate part in coding.

Another skill that I have gained from my previous entry is <b>consideration</b>, which is to consider the impact of what I create on my users. I gained this skill by coming up with ideas for my mini-game that will be appropriate to all age groups and enjoyable to everyone who wants to play it. This skill has also helped me realize which parts of my mini-game are necessary to include and which parts are not the best to include for a game being played by people from a wide range of ages. Additionally, having consideration helps me choose which prizes to give my users to make them more excited to play my mini-game and satisfied with the end result.

Lastly, I have gained the skill <b>creativity</b>, which is to think outside the box, be innovative, and create the future. I gained this skill by thinking of several different ways to make my mini-game as visually appealing as possible. I have experimented with different codes, colors, shapes, sizes, and more to make sure that I am creating a virtual setting that is both original and imaginative. I have also thought of different types of characters I would like to include in my mini-game, which was me using creativity to design avatars that are different from other games and can possibly resemble some of my users.

### Concluding Thoughts 
Overall, I feel that I understand my tool a lot more now after tinkering with it for the last couple of months. I am getting more comfortable with A-Frame and all the different guides it has in order for me to create the most effective mini-game. I will continue to use the knowledge I have gained from class and the skills I have gained throughout the process of completing my Freedom Project to make my mini-game more advanced, as well as using several strategies to make my code more well-developed. I plan to continue tinkering with my tool a bit more to soon be able to create a prototype that I can use to test out all of my ideas and see what I can improve on to allow my users to have the best experience playing my mini-game. 

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
