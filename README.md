<h1 align='center'>responsive design using css grid</h1>

<h2 >LEARNED</h2>
- learned about responsive grid frameworks
- learned the basics of 960GS and bootstrap, to see how frameworks operate and what theyre capable of
- learned basics of SASS preprocessor
- decided that I should learn grid more thoughly to create responsive layouts instead of frameworks

<h2 >GRID NOTES</h2>

<h3>Container</h3>
- display : grid / inline-grid
- grid-template-columns : specifies the number of columns
- grid-template-rows : specifies the number of rows
- grid-colums/rows : shorthand for grid-template-rows / grid-template-columns
- grid-area-name : specifies (by 'grid-area') where to place each child element
- grid-gap: shorthand for column-gap/row-gap. sets the size of the grid line
- justify-items: aligns all items in grid-item along the row axis
- align-items: aligns all items in grid-item along the column axis
- place-items: shorthand for justify-items/align-items
- justify-content / align-content: aligns grid within grid container, when the actual grid is small than the grid container
- place-content: shorthand for justify-content / align-content
- grid-auto-columns / grid-auto-rows: specifies auto generated grid-items when there are more grid-items than cells
- grid-auto-flow: controls how the auto-placement algorithm works

<h3>Child Properties</h3>
- grid-column-start / grid-column-end || grid-row-start / grid-row-end: states starting and ending lines for an individual grid-item
- grid-column / grid-row: shorthand for grid-column-start / grid-column-end || grid-row-start / grid-row-end
- grid-area: Gives an item a name so that it can be referenced by a template created with the grid-template-areas property. Alternatively, this property can be used as an even shorter shorthand for grid-row-start + grid-column-start + grid-row-end + grid-column-end.
- justify-self: Aligns a grid item inside a cell along the inline (row) axis
- align-self: Aligns a grid item inside a cell along the block (column) axis
- place-self: place-self sets both the align-self and justify-self properties in a single declaration.

<h3>Sizing Keywords</h3>

- min-content: the minimum size of the content. Imagine a line of text like “The very long hotdog.”, the min-content is likely the width of the world “The”.
- max-content: the maximum size of the content. Imagine the sentence above, the max-content is the length of the whole sentence.
- auto: this keyword is a lot like fr units, except that they “lose” the fight in sizing against fr units when allocating the remaining space.
- fit-content: use the space available, but never less than min-content and never more than max-content.
- fr: portion of the remaining space

<h3>Functions</h3>
- min-max: sets a minimum and maximum value for what the length is able to be
- min
- max
- repeat
-> auto-fill: Fit as many possible columns as possible on a row, even if they are empty.
-> auto-fit: Fit whatever columns there are into the space. Prefer expanding columns to fill space rather than empty columns.
-> ex: repeat(auto-fit, minmax(250px, 1fr))
