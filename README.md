# Data structures (DS) and Algorithms (A) 🧡💙💚💟💐❤️

- DS --> Various Methods we can use for Storing and Organising the DATA.
- A --> Various Steps we can follow to solve the problems with a minimum efficiency.

## Measure the Efficiency of the Algorithm

### Time Complexity
Amount of time required for the execution

![1__Time Complexity __O(1).png,1__Time Complexity __O(n).png,1__Time Complexity __O(n^2).png]

- when execution time is constant = Order of 1 (O[1])
- when execution time is not constant = Order of 1 (O[n]) --->  ```For``` Loops
- when execution time is not constant = Order of 1 (O[n^2]) --->  ```Nested For``` Loops

### Space Complexity
The amount of Memory Space needed when it runs

![1__Various DataTypes and Their Codes.png]

![1__Space Complexity __O(1).png,1__Space Complexity __O(n).png]
   - when space is constant = Order of 1 (O[1])
   - when space is not constant = Order of 1 (O[n]) --->  For Loops

## ✅ Methods of DS = Array
The array can help to stroke multiple elements in a single variable.

- Properties of Array:
  - Consisted only same data types
  - Have own index for all elements in the array which can help to access the elements


- Limitations:
  - We cannot store elements beyond the size of the array that we already defined size of the array.
    - So, if we want to add more elements to the array beyond the limit.
      - Then, we need to create a new array that can store new elements with a periods array.

### Types of Array
![1__Types of Array.png]
1. One-Dimensional (1D) Array --> a = [1,2,3]
2. Multi-Dimensional Array
      - 2-Dimensional (2D) Array 
      - 3-Dimensional (3D) Array

### Array Elements Represents in Memory
![Array Elements Represents in Memory]

- Array elements store in the memory without gaps between the elements.
- The Compiler is decided where elements are stored continuously.

### Create an Array
  - Time Complexity of Creating an array = O(1)
  - We can create:
    - empty array --> arr1 / 
    - filled with half amount of elements in the array --> arr2 / 
    - fully filled array -->  arr3.
    
![1__Create an Array.png]

![1__Various DataTypes and Their Codes.png]


### 1__Insert Elements to Array
![1__Insert Elements to Array.png]

- To End of the Array --> ```append(element)```
  - Time Complexity = O(1)
- To Anywhere in the Array --> ```insert(index of location, element)```
  - We need to shift elements to the right or left side.
  - Time Complexity = O(n)
- Add more element to the array --> ```extend([element1,element2,element3,element4])```

### 2__Traversal Operations in the Array
![1__Traversal Operations in the Array.png]
- We want to go through the all elements in the array. --> ```for```Loop
  - Time Complexity = O(n)

### 3__ Access Elements in Array
![1__Access Elements in Array.png]
- We don't need to go through every element.
  - using an index, we can access the elements immediately.
    - Time Complexity = O(1)

### 4__Delete an Element
![1__Delete an Element.png]
- Delete last element --> ```pop```
  - Time Complexity = O(1)
- Delete Anywhere in the Array --> ```remove```
  - We can't leave a gap between the array in memory.
  - Time Complexity = O(n)
  
      
## ✅ Methods of DS = Linked List
![2.1__Linked List_1.png]

- Linked List is combination of nodes which is consisted of value & Reference.
- There is no order.
- We can add and remove nodes.
- Using Reference in a Node, We can connect the node to another node.
- Why Head?
  - It is indicated that initialization of the linked list.
- Why Tail?
  - It is indicated that the end of the linked list.

### Linked List Represents in Memory
![2.2__Linked List Elements Represents in Memory]
![2.3__Array Elements Represents in Memory]

- Nodes are stored Randomly not like Array.
- In Array, we can access values quickly using an index. 
- But, in Linked List, we have to go through the all nodes until the needed node ( can't quickly access).

### Types of Linked List
1. Singly Linked List
- We Can go in Only One Direction.
- Can't go to 1st Node.
- In Music Player, we can go from song 1 to end. but can go 1st song by pressing ```>>```.

    ![2.4__Singly Linked List.png]

    ![2.5__Singly Linked List Music Player.png]

4. Circular Singly Linked List
- It is doing forward and also can go to 1st node.
- In music Player, we can go from 1 st song to the end and then again can go to 1st song by pressing ```>>```

    ![2.6__Circular Singly Linked List.png]

    ![2.7__Circular Singly Linked List Music Player.png]

5. Doubly Linked List
- In here, You can go forward and backward.
- In Music Player, 
  - ```>>``` --> 1st song to end 
  - ```<<``` --> end to 1st song

      ![2.9__Doubly Linked List.png]

      ![2.9__Doubly Linked List Music Player.png]

8. Circular Doubly Linked List
- In here, we can go forward and backward.
- and also, we can go directly to 1st node and end node.
- In Music Player, 
  - ```>>``` -->  1st song to end (1->2->3) `&` end to 1st song to directly (3->1)
  - ```<<``` -->  end song to 1st (3->2->1) `&` 1st to end song to directly (1->3)

       ![2.11__Circular Doubly Linked List.png]

       ![2.11__Circular Doubly Linked List Music Player.png]


### Array Vs Linked List

#### Memory Requirement
![2.12__Memory Requirement.png]

| Array                                                    | Linked List                                                                                          |
|----------------------------------------------------------|:-----------------------------------------------------------------------------------------------------|
| Store elements in memory continuously without gaps       | Nodes of LS store randomly in the memory.                                                            |
| Takes Minimum memory space.                              | Takes more space when storing because needs to store node's values and reference (pointer) variable. |
| Need to fix the size of the array at the initialization. | We don't need to define the size of LS.                                                              | 


#### Inserting an Element

###### At the Beginning
![2.13__Inserting_At the Beginning.png]

| Array                                | Linked List                                |
|--------------------------------------|:-------------------------------------------|
| Need to shift all elements to right. | Just add 1 node, No need to shift.         |
| Time Complexity = O(n)               | Time Complexity = O(1)                     |


###### At the End
![2.14__Inserting_At the End.png]

| Array                                               | Linked List                        |
|-----------------------------------------------------|:-----------------------------------|
| No Need to shift. Just add to the end of the array. | Just add 1 node to en before Tail. |
| Time Complexity = O(1)                              | Time Complexity = O(1)             |


#### Removing an Element

###### At the Beginning
![2.15__Removing_At the Beginning.png]

| Array                                                          | Linked List                                              |
|----------------------------------------------------------------|:---------------------------------------------------------|
| Need to shift all elements to left after removing 1st element. | No need to shift elements. Just changed the referencing. |
| Time Complexity = O(n)                                         | Time Complexity = O(1)                                   |


###### At the End
![2.16__Removing_At the End.png]

| Array                                        | Linked List                     |
|----------------------------------------------|:--------------------------------|
| Just remove element at the end of the array. | Just changed the referencing.   |
| Time Complexity = O(1)                       | Time Complexity = O(1)          |


#### Accessing an Element
![2.17__Accessing Elements.png]

| Array                                              | Linked List                                                                                                                                                       |
|----------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Have index number to accessed the element easily.  | We only know the Head and tail nodes. If you want to access the value, you have to go through the element from the Head node to until the goal using referencing. |
| Time Complexity = O(1)                             | Time Complexity = O(n)                                                                                                                                            |


### Operations on Linked List

![2.18__Operations LS.png]

#### 1. Creation 

![2.19__Creation a LS.png]

- Create a Head and Tail.
- Create a Node with Value & Reference.
- Connect node to Head & Tail.

#### 2. Traversal
![2.20__Traversal Linked List.png]

#### 3. Insertion

