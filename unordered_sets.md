# Unordered Sets

*unordered_set is an associative container that contains a set of unique objects of type Key. It is implemented using hash table that allows fast search for individual elements, based on their keys.*

## difference between set and unordered_set

*In unordered_set elements are not stored in sorted manner*


## declaration

```cpp
unordered_set<data_type> variable_name;
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    unordered_set<int> s = {4, 2, 3, 1, 5};
    for (auto it = s.begin(); it != s.end(); it++) {
        cout << *it << " ";
    }
}
```

#### output

```cpp
4 2 3 1 5
```

