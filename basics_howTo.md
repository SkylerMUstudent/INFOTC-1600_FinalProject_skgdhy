# Creating a SVG guide

Navigation:
 - [Home](README.md)
 - [How to create a SVG](basics_howTo.md)

 ------

 With this guide, we'll start off with how to create a basic SVG image.

 For this tutoral, we are going to create a Polygon!

 <svg width="500" height="300">
    <polygon points="150,15 258,77 258,202 150,265 42,202 42,77"
    style="fill:blue;stroke:darkred;stroke-width:5">
 </svg>

 To begin this tutoral, you will want to create a blank HTML file and a editor such as Visual Studio Code or any editor that supports HTML editing.

 After you created a HTML file we can work in, we'll begain by declaring a root element \<svg>.

 > \<svg>
 >
 > \</svg>

 Next we are going to add hight and width of the svg image.
 We are telling it we are going to have a width of 500 pixles wide by 300 pixles high.

 > \<svg width="500" height="300">
 >
 > \</svg>

 Nothing will appear yet, this simply creates the area where the SVG image takes up on the screen.

 Next, we are going ot declare the polygon points.
 > points
 
 The **points** attrubute works by telling it where we want to start drawing. It goes by X and Y points on the SVG image.
 
 So if we say something like **points="200,50"**, we are saying "Draw a point of the shape at **x(200),y(50)**". The points are messuared starting from the Top-Left of the SVG image.

 > \<svg width="500" height="300">
 >
 > \<polygon point="150,15">
 >
 > \</svg>

 From here, we are going to then give it more points to draw to.

 >\<svg width="500" height="300">
 >
 >   \<polygon points="150,15 258, 77 258,202 150,265">
 >
 > \</svg>

 <svg width="500" height="300">
    <polygon points="150,15 258,77 258,202 150,265">
 </svg>

Now we are starting to see something! But we are not finished yet. We still have to complete the shape.

>\<svg width="500" height="300">
>
>    \<polygon points="150,15 258,77 258,202 150,265 42,202 42,77">
>
> \</svg>

<svg width="500" height="300">
    <polygon points="150,15 258,77 258,202 150,265 42,202 42,77">
 </svg>

 So now we have our Polygon!

 What we went over was just drawing our shape, but now we migth want to add color.

> \<svg width="500" height="300">
>
>    \<polygon points="150,15 258,77 258,202 150,265 42,202 42,77"
>    style="fill:blue;>
>
> \</svg>

<svg width="500" height="300">
    <polygon points="150,15 258,77 258,202 150,265 42,202 42,77"
    style="fill:blue;">
 </svg>

 We know have a blue polygon!
 
 We now know how to draw our shapes and color them. But I think we can do a little more to help this shape *"pop"* out a little more!

 We are now going to add a stroke on the boarder of our polygon.

> \<svg width="500" height="300">
>
>    \<polygon points="150,15 258,77 258,202 150,265 42,202 42,77"
>    style="fill:blue;
 stroke:darkred;">
> 
> \</svg>

<svg width="500" height="300">
    <polygon points="150,15 258,77 258,202 150,265 42,202 42,77"
    style="fill:blue;stroke:darkred">
 </svg>

 We now have a darkread stroke on our polygon, but its somewhat hard to see, so now we are going to inlarge the strock so it is more thick.

 This will help the polygon have boarders that are easier to see. If you are desiging a image, its important to take what background the user might see. If they are looking at a white background, its important not to use colors too bright that it hides the shape. The same can be said for dark backgrounds. The idea is to make sure the user is able to veiw your image.

> \<svg width="500" height="300">
>
>    \<polygon points="150,15 258,77 258,202 150,265 42,202 42,77"
    style="fill:blue;stroke:darkred;stroke-width:5">
>    
> \</svg>

 <svg width="500" height="300">
    <polygon points="150,15 258,77 258,202 150,265 42,202 42,77"
    style="fill:blue;stroke:darkred;stroke-width:5">
 </svg>

 And we are DONE!

 This was just a very basic way to design a SVG image. There are MANY different ways to create SVGs. 

 Now you know how to create one, but there are many different styles and tricks you can do with SVGs!

 Here are a few other different SVGs that can also be created!

 -------
 ## Other kinds of SVGs

 <svg height="100" width="100" xmlns="http://www.w3.org/2000/svg">
  <circle r="45" cx="50" cy="50" fill="red" />
</svg>

<svg width="400" height="300">
            <path d="M 150 0 L75 200" fill="none" stroke="black" stroke-width="0.5"></path>
            <path d="M 175 0 L74 180" fill="none" stroke="black" stroke-width="1"></path>
            <path d="M 210 0 L72 160" fill="none" stroke="black" stroke-width="2"></path>
            <path d="M 250 0 L70 140" fill="none" stroke="gray" stroke-width="3"></path>
            <path d="M 300 0 L68 120" fill="none" stroke="gray" stroke-width="4"></path>
            <path d="M 370 0 L64 100" fill="none" stroke="gray" stroke-width="5"></path>
        </svg>

<svg height="250" width="350" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <marker id="circle" markerWidth="8" markerHeight="8" refX="5" refY="5">
      <circle cx="5" cy="5" r="3" fill="black" />
    </marker>
    <marker id="arrow" markerWidth="10" markerHeight="10" refX="5" refY="5" orient="auto">
      <path d="M 0 0 L 10 5 L 0 10 z" fill="black" />
    </marker>
  </defs>
  <line x1="10" y1="10" x2="300" y2="200" stroke="red" stroke-width="3" marker-start="url(#circle)" marker-end="url(#arrow)" />
</svg>

<svg height="210" width="500" xmlns="http://www.w3.org/2000/svg">
  <polygon points="100,10 40,198 190,78 10,78 160,198" fill="lime" fill-rule="evenodd" />
</svg>

<svg height="150" width="400" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <radialGradient id="grad1" cx="50%" cy="50%" r="50%" fx="50%" fy="50%">
      <stop offset="0%" stop-color="red" />
      <stop offset="100%" stop-color="blue" />
    </radialGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
</svg>

<svg width="200" height="180" xmlns="http://www.w3.org/2000/svg">
  <rect x="30" y="30" height="110" width="110" style="stroke:green;fill:red">
    <animateTransform
      attributeName="transform"
      begin="0s"
      dur="10s"
      type="rotate"
      from="0 85 85"
      to="360 85 85"
      repeatCount="indefinite" />
  </rect>
</svg>