# d3-flextree-v4

This is a copy of the [d3-flextree](https://github.com/klortho/d3-flextree) D3 plugin
updated to be compatible with version 4 of D3.

## Usage

This library operates on [`d3-hierarchy`](https://github.com/d3/d3-hierarchy#hierarchy) objects. Its API is similar to [`d3.tree`](https://github.com/d3/d3-hierarchy#tree), the main difference being that `nodeSize()` also accepts a function that will be called for each node.

```js
const flextree = require('d3-flextree-v4');
const tree = flextree().nodeSize((node) => {
  return [
    node.data.width,
    node.data.height
  ];
});

flextree(hierarchy); // adds "x" and "y" properties for each node.

```
