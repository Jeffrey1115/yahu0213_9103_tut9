## Instructions on how to interact with the work

When interacting with the work, you can move elements on the screen by dragging the mouse. The color of each element will change randomly every two seconds, and when dragged, the element will move to the top layer of the screen. By clicking and dragging the elements, you can see their changes in the animation.

## Details of your individual approach to animating the group code

1. Which did you choose to drive your individual code: audio, interaction, Perlin noise or time.

   I chose to use timer and event to drive my personal code. By setting time intervals and event triggers, I achieved animations of graphical colors, positions, and timing.

2. Which properties of the image will be animated and how; highlighting how it is unique from other group members (i.e. one changes colours, the other component sizes, another reveals only some components at a time, etc.). You will need to work with your group members to make sure your work is sufficiently different from each other.

   My animations are primarily based on changes in color and position, controlled by timer and event.

3. References to inspiration for animating your individual code; these can be images (still or gifs). How did they influence your submission?

   My animation inspiration comes from the personal experience of appreciating artworks. Each person's mood differs, resulting in different perceptions, much like how 1000 people can have 1000 different feelings about the same artwork. I aim to create animations that reflect these varied moods based on the artist's original ideas.

4. A short technical explanation of how your individual code works to animate the image and any appropriate references.

   1. During the initial rendering, each element is sequentially loaded into the squares array. Then, setInterval is used to randomly select a new color for each child element every two seconds.


   2. During each update cycle of the interface, the lerp() function is used to transition each child element from the old color to the new color.
   
   3. When dragging, a variable called draggedElement binds to the currently dragged element. In the mousePressed event, this element is removed from the squares array and added to the end of the array to bring it to the top layer. In the mouseReleased event, the binding of draggedElement to the element is canceled.
