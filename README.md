# CPP-STL

## 1. STL

STL is a C++ library that provides four components:

- Containers
- Algorithms
- Iterators
- Functions

## 2. Containers

*Containers are used to store data. They are objects that hold data and provide a way to access it. The data is stored in a container in a specific format. The format depends on the type of container. The data can be accessed using iterators.*

### 2.1. Sequence Containers

*Sequence containers are used to store data in a linear sequence. The data is stored in a specific order. The order is maintained by the sequence of elements. The elements are accessed by their position in the sequence. The elements are accessed using iterators.*

#### 2.1.1. [Vector](vector.md)

*Vectors are sequence containers representing arrays that can change in size.*

#### 2.1.2. List

*Lists are sequence containers that allow non-contiguous memory allocation. As compared to vectors, lists perform better in inserting, extracting and moving elements in any position within the container for which an iterator has already been obtained, and therefore also in algorithms that make intensive use of these, like sorting algorithms.*

#### 2.1.3. Deque

*Deque is an abbreviation of double-ended queue. They are sequence containers with the feature of expansion and contraction on both the ends. They are similar to vectors, but are more efficient in case of insertion and deletion of elements at the beginning or the end of the sequence.*

#### 2.1.4. Forward List

*Forward lists are sequence containers that allow non-contiguous memory allocation. As compared to lists, forward lists perform better in inserting and removing elements from anywhere in the container, and therefore also in algorithms that make intensive use of these, like sorting algorithms.*

#### 2.1.5. Array

*Arrays are sequence containers that encapsulate fixed size arrays. They are implemented as fixed size arrays which are placed directly in the storage space allocated to the container, which is generally on the stack.*

### 2.2. Container Adaptors

*Container adaptors are classes that use an encapsulated object of a specific container class as its underlying container, providing a specific set of member functions to access its elements. Elements are pushed into the specific container from the specific set of member functions.*


### 2.3. Associative Containers

*Associative containers are containers that store elements formed by a combination of a key value and a mapped value, following a specific order. The value of the mapped value can be accessed directly by its corresponding key value and, in some cases, by the iterators to these values, and keys can be retrieved from the values.*


### 2.4. Unordered Associative Containers

*Unordered associative containers are containers that store elements formed by the combination of a key value and a mapped value, and which allows for fast retrieval of individual elements based on their keys.*


## 3. Algorithms

*Algorithms are a collection of functions that perform specific operations on ranges of elements.*

## 4. Iterators

*Iterators are objects that point to elements in a range. They are used to access the elements of a container. Iterators are used to point to the beginning and the end of a range of elements. They are used to access the elements of a container. Iterators are used to point to the beginning and the end of a range of elements.*

## 5. Functions

*Functions are objects that can be called like functions. They are used to perform operations on a range of elements. They are used to perform operations on a range of elements.*


