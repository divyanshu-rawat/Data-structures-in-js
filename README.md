# Data-structures-in-js

### TREES
* Abstract data type
* General Tree:
  * A tree has a root node.
  * The root node has 0 or more children.
  *Each child node has 0 or more children.
  (each node in the tree can be seen as a subtree)
*Constraints:
  * A child has only one parent and the root node has no parent.
Note: A tree is a special type of graph. A tree is a graph without cycles.
* Operations:
  * tree.addChild(value)
=> child node (new tree)
add child to tree/subtree and return child node (which should be a tree instance)
  * tree.contains(value)
=> true/false
Return true if value is in tree, false if not
  * tree.traverseDepthFirst(callback)
=> undefined
Invoke the callback for every node in a depth-first order
  * tree.traverseBreadthFirst(callback)
=> undefined
Invoke the callback for every node in a breadth-first order
```
function Tree (value) {
  // implement me...
}

Tree.prototype.addChild = function(value) {
  // implement me...
};
// Time complexity:


Tree.prototype.contains = function(value) {
  // implement me...
};
// Time complexity:


Tree.prototype.traverseDepthFirst = function(fn) {
  // implement me...
};
// Time complexity:


Tree.prototype.traverseBreadthFirst = function(fn) {
  // implement me...
};
// Time complexity:
```



## HEAPS
* Abstract data type
 *A max heap is a special type of binary tree that satisfies two properties:
 * 1. Shape property – All nodes which are at the same depth of the tree from the root node are said to be on the same level. Each level of a max heap must be filled with nodes before any nodes can appear on the next level of the max heap. When nodes are added to the next level of the max heap they must be added from left to right.
 * 2. Heap property – In a max heap all nodes are greater than or equal to each of its children nodes.
Heaps are usually implemented in an array. The first element is the root, the next two are the children of the root, and the next four are their children. The children of the node at position n are at positions 2n+1 and 2n+2.
View visualization here: https://presentpath.github.io/heap-visualizer/
* Operations:
 * heap.insert(value)
=> undefined
Add value to heap according to the shape and heap property
 * heap.removeMax()
=> max value
Remove the max value from the heap, reorder the heap, and return the max value



## SET
* Abstract data type
 * Stores unique values in no particular order
 * No mechanism for retrieving elements
 * Your set should be able to store any JavaScript primitive
* Operations:
 * mySet.count()
=> integer value for the number of values present in set
 * mySet.add(value)
=> set object
 * mySet.delete(value)
=> true if value was present and removed
=> false if value was not present
 * mySet.has(value)
=> true/false
 * mySet.forEach(callbackFn)
=> no return value
calls callbackFn once for each value in the set
Note: ES6 has a Set data structure as part of the core language.
```
function Set(capacity) {
  // implement me...
}

Set.prototype.count = function() {
  // implement me...
};
// Time complexity:

Set.prototype.add = function(value) {
  // implement me...
};
// Time complexity:

Set.prototype.delete = function(value) {
  // implement me...
};
// Time complexity:

Set.prototype.has = function(value) {
  // implement me...
};
// Time complexity:

Set.prototype.forEach = function(callback) {
  // implement me...
};
// Time complexity:
```







feel free to add more
