In 
.gallery {
  width: 100%;
  max-width: 350px;
}

Your images are too big. Create a .gallery img selector to target them. Give them all a width of 100% and a max-width of 350px so they shrink as needed but don't get too big.

![image](https://user-images.githubusercontent.com/115179685/200230907-deecd640-bc61-4fb7-ae97-0ead79e8f4e5.png)
![image](https://user-images.githubusercontent.com/115179685/200230979-efbe2d75-7c0a-494f-aa7c-8153ecc57c82.png)
![image](https://user-images.githubusercontent.com/115179685/200231032-4d188716-5c44-48ee-8113-0eafb72ebc08.png)
![image](https://user-images.githubusercontent.com/115179685/200230637-9c79ba3a-c355-43dd-8956-90d8a25c5591.png)
![image](https://user-images.githubusercontent.com/115179685/200230709-db2416af-fe93-4886-a35d-a9967dfded7d.png)


# Flexbox is a one-dimensional CSS layout that can control the way items are spaced out and aligned within a container.

When images are too big. Give them all a width of 100% and a max-width of 350px so they shrink as needed but don't get too big.

.gallery img {
    width: 100%;       //to fit the 100% in the cointainer 
    height: 300;       //to keep unifrom on imgs
    max-width: 350px;  //  for shrink as needed despite screen width, it allowed a uniform re-sizing in the pics 
}

# Flexbox has a main and cross axis. The main axis is defined by the flex-direction property, which has four possible values:

row (default): horizontal axis with flex items from left to right
row-reverse: horizontal axis with flex items from right to left
column: vertical axis with flex items from top to bottom
column-reverse: vertical axis with flex items from bottom to top

Note: The axes and directions will be different depending on the text direction. 

# The flex-wrap property determines how your flex items behave when the flex container is too small. Setting it to wrap will allow the items to wrap to the next row or column. nowrap (default) will prevent your items from wrapping and shrink them if needed.

# The justify-content property determines how the items inside a flex container are positioned along the main axis, affecting their position and the space around them.

# The align-items property positions the flex content along the cross axis. In this case, with your flex-direction set to row, your cross axis would be vertical.

# *** Images have different aspect ratios (distorted). Rather than setting each aspect ratio individually, you can use the object-fit property to determine how images should behave. Give your .gallery img selector the "object-fit" property and set it to cover. This will tell the image to fill the img container while maintaining aspect ratio, resulting in cropping to fit. ***
 
# The gap CSS shorthand property sets the gaps, also knowns as gutters, between rows and columns. The gap property and its row-gap and column-gap sub-properties provide this functionality for flex, grid, and multi-column layout. 

# The ::after pseudo-element creates an element that is the last child of the selected element. You can use it to add an empty element after the last image. If you give it the same width as the images it will push the last image to the left when the gallery is in a two-column layout. Right now, it is in the center because you set justify-content: center on the flex container.