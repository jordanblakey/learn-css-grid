# Learn CSS Grid

**Notes and Exercises using basic CSS Grid functionality**

## Basic Syntax

### Columns

```css
display: grid;
```

Render the current element as a grid.

```css
grid-template-columns: 20% 30% 50%;
/* Percentage widths */

grid-template-columns: 1fr 1fr 1fr;
/* Fractional units */

grid-template-columns: repeat(3, 1fr 2fr);
/* Repeat function takes an iteration count per row, and x fractional widths to be repeated. This example produces rows of six elements with widths 1:2:1:2:1:2 */

grid-column-gap: 10px;
/* define a dynamic column gutter */
```

Define the number of grid columns in the current element.

### Rows

```css
grid-auto-rows: 200px;
/* All rows will have height of 200px. */

grid-auto-rows: minmax(200px, auto);
/* Set a minimum and maxiumum height using the minmax() function */

grid-template-rows: 200px 300px 400px 200px;
/* manually set the height of each row */

grid-template-rows: repeat(10, minmax(200px, auto)) 200px;
/* use repeat, minmax to handle variability in content. */

grid-row-gap: 10px;
/* define a dynamic row gutter */
```
