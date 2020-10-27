## User Manual
Installing the application: Download the zip file, open the project in an editor, and run “npm install” to download and install all of the necessary packages. To run the web-app locally, simply run “npm start” in your terminal. 

_**Draw Mode**_: when the “Draw” button is pressed (the app is already defaulted to Draw Mode), users can draw rectangles of any shape and size, within the left pane. The mouse needs to be held down between the start and end points. Zero width and zero height boxes are not allowed.

_**Grab Mode**_: when the “Grab” button is pressed, users will not be able to draw any shapes. Instead, by clicking on a shape, users can move it around, within the left pain. By clicking and dragging on one of the 8 selection handles that appear on a highlighted element, users can resize a shape in the direction of the handle. To deselect and element, click on the canvas.
When in Grab Mode, users can also change the fill and stroke color, as well as the stroke thickness and corner radius (“roundness”) of the selected rectangle. Note - clicking on a rectangle will change the slider values to reflect the values of the selected shape.
Only when a shape is selected in Grab Mode it can be deleted by clicking the “delete” button that appears in the right pane, and deleting the shape. 

_**Undo, Redo, Clear**_: this app allows the user to undo and redo the creation of shapes. The undo/redo buttons can only remove and put back elements into the left pane. Reverting a change in color, size, line thickness, etc. is not possible at this moment. Note that the “delete” button cannot be undone. 

## Implementation
This project was mplemented with Javascript and React. I used node-sass to make it SCSS compatible. I used an Immutable.JS library to have more robust, persistent, immutable data structures. I used “react-color,” an npm-package, to auto-generate color sliders for me. I also used the chrome React Dev Tools add-on for state management and debugging. I used one main reference for how to use the SVG "path" object to draw lines on a page. I listed this at the top of the file. From there, I extrapolated the information in the sample code to work for SVG "rect” object, which I learned the basic syntax for by visiting the W3 website.

## Future Enhancement
This was a great exercise in empathizing with the toolmakers of some of my favorite platforms, like Figma, Sketch, and others. I realize now how much planning it takes to create tools that can generate shapes of any size, have the shapes be aware of each other and behave in smart ways, and do this all with a great user experience. 

In the future, I would like to create a more generic way to create shapes, put bounding boxes around them, and create ways to resize and edit them. The methods I've used in this project are fairly limited to just modifying rectangles. I'd love to explore how to make this more generalizable for all kinds of shapes. I'd also like to explore how to manage shape hierarchies, to truly make this tool more useful than just drawing single layer shapes of any size and color. The ability to nest objects within each other, modify the indexes, and make meaningful objects, would make this tool much more useful. 
