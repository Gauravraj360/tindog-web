
# A Tindog website - Under the guidance of Angela Yu
This is my first responsive website. It is a dummy project that I have learned while the training of web development under the mentorship of Angela Yu co-founder of App brewery. 

## Table of contents

  - [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
  - [Acknowledgments](#acknowledgments)

  ## Overview
    This is a Tindog website specially made buying dogs. We can actually find here stuff related to dogs and also find a partener for dogs.

  ### Screenshot

  ### Links
    - Solution URL: (https://github.com/Gauravraj360/tindog-web)
    - Live Site URL: (https://gauravraj360.github.io/tindog-web/)

  ## My process

  I started making this project few days back and I constantly give my time on this project and following my mentor and actually something in this project was bit hard to grasp but I took time and practise all the little stuff like positioning with z-index , selectors combination in css and also learned how to refactor our code. I used bootstrap as a framework here that made my things easy as it has library of different types of things. Few of things I used here is navigation bar and download buttons and also i make grids with bootstrap.
  I have learned many things and will learn a lot things ahead.

  ### Built with

  - Semantic HTML markup
  - CSS3 custom properties
  - Bootstrap5.2.0
 
 # What I learned

 I learned many things while making this project few of things I mentioned down.

 - priority of CSS styling 
    Inline - It is written in the tags only like <h1 style=width:5px;>
    Internal- It is written inside the body like <style> h3{ width: 5px;} </style>
    External - It is written in a file with extension .css  witten like h1{height: 200px; } 
    * priority of these styling is top to down but best coding practice is to do external styling because it is to modify and read

 - use of class and ids
    class syntax is .div and we can use this if we have common class or groups in our code
    Id syntax is #title and we can use this for a specific part simply say Ids are identifying tag use for something unique like a section of our code let say title section
    (here div and title is just for example basically i m refering to . & #)
    Pseudo class- It is use to implement another property to same class. eg - to hover over a icon let say we have a class icon to apply any hovering feature we can write feature like .icon:hover{ features }

 -  The Box Model
    Everything in the html is nothing but a box and each box has some margin & border.
    I have learned about margin , border & padding.
    Margin- it provides space b/w two boxes.
    Border- provides border to a box.
    Padding- increases size of the box. It provide extra space b/w box and its element.
    * there is lot of learning in this box concept that i can't just write here as more u used to it you will learn about it.

 - Display property of CSS
    1. Block - It block other element to sitting next to it. eg. <p>,<h>,<div>,<ol>,<ul> ,<li>.
    2. Inline - It does not block other element to sit beside them but we can't change it's width. eg <span>, <img>, <a>.
    3. Inline-Block - It allow element to sit beside them as well as to change it's width. 
    4. None - It do nothing to the element. but it's important bcs we can make any of the above display property to none just by (display: none;) 
    * we can also make any element to any display property eg display: inline/block/inline-block.
 
 - Children Sits on Parents
    This property actually means that a child class is always gonna take first effect on screen, parent will be beneath child.
    and also if same property to a element is write twice the one who is written later is the one who will be prioritized.

 - position
   1. static- all html elements are static in their position by default.
   2.  Relative- this allow us to position the element that we select relative to how it would have been positioned when it had been static.( works like a coordinate system in mathematics )
   3. Absolute- It allow to position a block anywhere relative to it's parents whose position is relative but it affect the position of other element around it.
   4. Fixed- It will make the position of the element fixed to a place even we scroll down it will be fixed on a particular place on screen. It is really helpful to make navigation bars.

 - Use of % ,em, & rem over px
   we can use %, em & rem if we want to make change related to body means the size of things will be affect if the size of body affects.
   px is something fixed size that will not change with the screen size.
   difference b/w em & rem - rem means it will change the size of the element ignoring the root values applied.

 - learned about floating & clear property
   float- make change to float element around another element.
   clear- it actually clear the floating part but make sure the alignment does not go beyond right/left.
   * we don't usually use floating property there is some better property than this.

 - z-indexing
   z-index -> actually position the element in z-direction means it will keep the element in the z-direction up or down.
   * we must have to order the stacks by using position absolute ,relative or fixed.
   ```html
        <body>
            <div class="box1" >
                Red
            </div>
            <div class="box2">
                yellow
            </div>
            <div class="box3">
                blue
            </div>
        </body>
   ```
   ```css
       .box1,.box2,.box3{
            height:200px;
            width:200px;
            position:absolute;
        }
        .box1{
            background-color:red;
          z-index:2;
        }
         .box2{
            background-color:yellow;
            left:20px;
            top:20px;
           z-index:1;
        }
         .box3{
            background-color:blue;
            left:40px;
            top:40px;
           
        }
   ```
   You can see that even the flow of code is written like blue should be on top of above but we can explicitly using z-index changes the order of stack and here red is on top.

 - I have learned bootstrap in this project some of the bootstrap predefined classes & ids that i use is :-
  1. navbar
   ```html
      <nav class="navbar navbar-expand-lg navbar-dark">
        <a class="navbar-brand" href="">heading</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02"
          aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse " id="navbarTogglerDemo02">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link p-4" href="#footer">example1</a>
            </li>
            <li class="nav-item">
              <a class="nav-link p-4" href="#pricing">example2</a>
            </li>
            <li class="nav-item">
              <a class="nav-link p-4" href="#cta">example3</a>
            </li>
          </ul>
        </div>
      </nav>
      ```
 2. Grid feature of bootstrap
   In this we can make grid layout just by using the predefine class property of bootstrap i.e raw & col
```html
<body>
<div class="row">
    <div class="col" style="background-color:red; border: 1px solid;">
        col
    </div>
    <div class="col" style="background-color:red; border: 1px solid;">
        col
    </div>
</div>

<div class="row">
    <div class="col-6" style="background-color:green; border: 1px solid">
        col-6
    </div>
    <div class="col-6" style="background-color:green; border: 1px solid">
        col-6
    </div>
</div>

<div class="row">
    <div class="col-lg-4 col-md-6 col-sm-6" style="background-color:yellow; border: 1px solid">
        col-lg-3 col-md-4 col-sm-6
    </div>
    <div class="col-lg-4 col-md-6 col-sm-6" style="background-color:yellow; border: 1px solid">
        col-lg-3 col-md-4 col-sm-6
    </div>
    <div class="col-lg-4 col-md-6 col-sm-6" style="background-color:yellow; border: 1px solid">
        col-lg-3 col-md-4 col-sm-6
    </div>
   </div>

<div class="row">
    <div class="col-lg-4 col-md-6 col-sm-12"style="background-color:grey; border: 1px solid" >
        A
    </div>
    <div class="col-lg-4 col-md-6 col-sm-12"style="background-color:grey; border: 1px solid" >
        B
    </div>
  
</div>
</body>
```
3. making Cards and grouping them

```html
 <div class="card" >
          <div class="card-header">
            <h3>card-header</h3>
          </div>
          <div class="card-body">
            <h2 class="price">body</h2>
            <p>example1</p>
            <p>example2</p>
            <p>example3</p>
            <div class="d-grid">
            <button type="button" class="btn btn-lg btn-outline-dark ">Sign Up</button>
          </div>
          </div>
      </div>
```

4. creating buttons
  ```html
  <button type="button" class="btn btn-primary" disabled>Primary button</button>
<button type="button" class="btn btn-secondary" disabled>Button</button>
<button type="button" class="btn btn-outline-primary" disabled>Primary button</button>
<button type="button" class="btn btn-outline-secondary" disabled>Button</button>
```
5. Making Slides using carousel class 

```html
<div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="..." class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="..." class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="..." class="d-block w-100" alt="...">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
```
- Learned small features like rotating an image
   syntax - transform: rotate(angle in digit);

 - Learned how to use predefined classes of bootstrap like section & container, Headers & footers.

 - Learned how to refactor our code
   As when we write a big piece of code 
   its very important to arrange them in order and write everything specifically 
   4 factor of refactoring 
   1. Readibility - easy to understand
   2. Modularity- easy to reuse
   3. Effieciency - how fast your code run
   4. Length - as short as possible (don't repeat yourself)

- Learned to combine selectors in CSS
    eg  #title .container{

    }

So basically I have listed down aprox everything I learned and there are more things to learn. 
So keep learning

### Useful resources

- [w3schools](https://w3-schools.com)
- [codepen]
- [codeply]
- [mdnDocs]
- [devDocs]
- [getBootstrap]
- [font-awesome]
- [flaticons]
- [dribble]
- [sneakpeak]
- [font.google.com]


## Acknowledgments
 
    I want to give credit to my mentor Angela Yu for her mentorship. I am really thankful to her that she guides us in all way to teach us the concept very clearly. This project give me some challanges and I learned many things throughout the journey. I also thankful to the useful resources  and documentation that is open to all of us some of them is w3school , mdn Doc , dev Doc , & also the community stackOverFlow.
