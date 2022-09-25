# grid-color-challenge

## Problem Statement

Create a 3x3 grid of tiles. When a tile is clicked it should change it's background color form white to red. 
If all tiles have been turned red, the individual tiles should change it's background color back to white in the order that they were clicked.

## My Implementation

- Use CSS flex box to create a 3x3 grid of div elements.
- Give each tile a data attribute of id 0-9
- Initailize empty array 'queue'
- Add a click event listener to the document that...
  - Returns if the event target has a data attribute id
  - Returns if the event target already exists in the 'queue'
  - Push the event target into to 'queue'
  - Check if the 'queue' is full (all tiles have been clicked)
 - Once all tiles have been clicked 
  - Set an interval that checks if items remain in the 'queue'
  - Uses shift() to remove and style the last item in the array
