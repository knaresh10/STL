# Unordered_map

*unordered_map is an associative container that contains key-value pairs with unique keys. It is implemented using hash table that allows fast search for individual elements, based on their keys.*

## difference between map and unordered_map

*In unordered_map elements are not stored in sorted manner*


## declaration

```cpp
unordered_map<data_type1, data_type2> variable_name;
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    unordered_map<int, int> m = {
        {3, 30},
        {1, 10},
        {5, 50},
        {2, 20},
        {4, 40}
    }
    for (auto it = m.begin(); it != m.end(); it++) {
        cout << it->first << " " << it->second << endl;
    }
}
```

#### output

```cpp
3 30
1 10
5 50
2 20
4 40
```


