# CSS grid children placement

# Lines

Add 1 `fr` to `.container`'s `grid-template-rows`.

Placing an element in a grid works by specifying not the row and column, but the _lines_. A 3x3 grid has four columns and four rows. They both start at 1.

Example:

```css
.six {
  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 3;
  grid-row-end: 4;
}
```

A somewhat simpler way to place an element is to use the `grid-column` and `grid-row` properties.

This example achieves the same result as the previous example:

```css
grid-column: 2 / 3;
grid-row: 3 / 4;
```

# Areas

Another way to place items in a grid is to use the `grid-area` property. This is mostly useful for positioning elements in a page layout.

Remove one `1fr` from `.container` so there are two rows again.
Add the following to the `.container`:

```
grid-template-areas: "one two three"
                     "four five six";
```

Now add two new classes:

```css
.five {
  grid-area: six;
}

.six {
  grid-area: five;
}
```
