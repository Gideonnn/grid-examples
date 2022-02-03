# CSS grid rows and columns

## Define the grid

To make a container div a grid we add `display: grid;` to it. This will change nothing, until you define the rows and columns.

## Define the rows

We use `grid-template-rows` to define the rows. Add `grid-template-rows: 1fr 1fr;` to the container div.

This defined two rows, the first row is 1fr and the second row is 1fr. These are `fraction units`, which work similar to flexbox values.

## Define the columns

Add `grid-template-columns: 1fr 1fr 1fr;` to the container div.

Now we see something happening. The elements are autmatically placed in the columns based on the source order.
