# d3Udemy

Code files available on [github](https://github.com/adamjanes/udemy-d3)

Went down a wee rabbit hole with TSV files. Found an [article on Stack Overflow](https://stackoverflow.com/questions/36814642/visual-studio-code-convert-spaces-to-tabs) that sorted me out.

## Section 24

Don't know where else to put this. Instructor says this defines the "standard setup for our SVG canvas."

```javascript
const MARGIN = { LEFT: 10, RIGHT: 10, TOP: 10, BOTTOM: 10 };
const WIDTH = 960 - MARGIN.LEFT - MARGIN.RIGHT;
const HEIGHT = 500 - MARGIN.TOP - MARGIN.BOTTOM;

const g = d3
  .select('#chart-area')
  .append('svg')
  .attr('width', WIDTH + MARGIN.LEFT + MARGIN.RIGHT)
  .attr('height', HEIGHT + MARGIN.TOP + MARGIN.BOTTOM)
  .append('g')
  .attr('transform', `translate(${MARGIN.LEFT}, ${MARGIN.TOP})`);
```
