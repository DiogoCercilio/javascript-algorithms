# Heap (data-structure)

- A Tree Based data structure, used when we want to be able to access the maximum or minimum element very quickly
- Sometimes Heaps are called Binary Heaps, and they are nearly complete Binary Trees
- Because we know that Heaps are nearly Binary Tree, the height of a Heap is O(logn) 
- There are multiple types of Heaps (Binary Heap, Fibonacci Heap, Binomial Heap, Pairing Heap)
- A good example of its implementation is using an Array. Ex:

```js
      20
     /  \
   10    15
  /        \
 5          3       =    [20, 10, 15, 5, 3]
```

Uses of Heaps includes:
- HeapSort (it uses max-heap)
- Dijkstra's algorithm (Finding the shortest path)
- Priority Queues (it uses min-heap)

There are two kinds of Heaps. Min Heaps and Max Heaps

## Max heap
- The value of i should be <= value of parent

## Min heap
- The value of i should be >= value of parent
- The root Node will be the very smallest element
- The elements are all smaller than their children
- When looking down the heap, the elements get bigger and bigger and bigger.



### Insertion
- The insertion element always goes in the next empty spot looking top to bottom, left to right
- We should insert the element as described below, and than bubble it up until we get the right spot
- We should compare the element with its parent. If it's out of the order, we swap them and keep going up the tree in this process

### Deleting
- We should get the last child slot, and then pu it on the root slot. After it, we should compare this slot with its children, and move it
until we don't have any bigger value (or less value, depending if it's a min-heap or a max-heap).
## Max heap


##### UseCases #####
...
##### Pros #####
...
##### Cons #####
...

In computer science, a **heap** is a specialized tree-based
data structure that satisfies the heap property described
below.

In a *min heap*, if `P` is a parent node of `C`, then the
key (the value) of `P` is less than or equal to the
key of `C`.

![MinHeap](./images/min-heap.jpeg)

In a *max heap*, the key of `P` is greater than or equal
to the key of `C`

![MaxHeap](./images/max-heap.jpeg)

![Array Representation](./images/array-representation.jpeg)

The node at the "top" of the heap with no parents is
called the root node.

## References

- [Wikipedia](https://en.wikipedia.org/wiki/Heap_(data_structure))
- [YouTube](https://www.youtube.com/watch?v=t0Cq6tVNRBA&index=5&t=0s&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)
