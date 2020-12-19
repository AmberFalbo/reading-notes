# 401 Notes-05: Linked Lists
[Back to 401 Index](401-index.md)<br>

## [Linked Lists](https://canvas.instructure.com/courses/2440726/discussion_topics/10225262)

### A Linked List is a sequence of `Nodes` that are connected/linked to each other. The most defining feature of a Linked List is that each `Node` references the next `Node` in the link.

### There are two types of Linked List - Singly and Doubly.

## Terminology:

1. ***Linked List*** - A data structure that contains nodes that links/point to the next node in the list. 
2. ***Singly*** - Singly refers to the number of references the node has. A `Singly` linked list means that there is only one reference, and the reference points to the `Next` node in a linked list.
3. ***Doubly*** - Doubly refers to three being two (double) references within the node. A `Doubly` linked list means that there is a reference to both the `Next` and `Previous` node.
4. ***Node*** - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
5. ***Next*** - Each node contains a property called `Next`. This property contains the reference to the next node.
6. ***Head*** - The Head is a reference type of type `Node` to the first node in a linked list.
7. ***Current*** - The `Current` reference is a reference type of type `Node` that is currently being looked at. This node is traditionally used when traversing through a full liked list. When traversing, You typically reste the current to the head to guarantee you are starting from the beginning of the linked list. 





## [What's a Linked List, Anyway pt1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)







## [What's a Linked List, Anyway pt2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)



Part's I'm trying to wrap around most.

Every Node has 2 parts:
`data` and a pointer to the `next` Node

Linked Lists is a collection of Nodes. 
The fist Node is always the Root Node and we keep a pointer on the root node in the list. The very last node doesn't have a Next, instead it's more like a null. 

Operations:
get_size()
find (data)
add(data) -- add to the beginning and change the root and use the next pointer to go to the next.
remove (data) -- find and locate the data looking for and cut off the next. The previous next links with the one that was after the one removed.

When making a class Node you need self, d(data), n(next) all = to none. 
Need your getters and setters.

The class LinkedList needs a dunder init. 
  - get_size, add, remove, find.
  - you need to account for changing the pointers around. And give a response for what happens.

MyList = LinkedList 

I got some information from the reading and videos as well since it's easier to do audio and visuals for my learning :-)







[Back to 401 Index](401-index.md)