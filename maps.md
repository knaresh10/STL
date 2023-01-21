# Maps

## Introduction

maps in cpp are associative containers that store elements in a mapped fashion. Each element has a key value and a mapped value. No two mapped values can have same key values.

## declaration

```cpp
map<data_type1, data_type2> variable_name;
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    map<int, int> m;
    m[1] = 10;
    m[2] = 20;
    m[3] = 30;
    m[4] = 40;
    m[5] = 50;
    for (auto it = m.begin(); it != m.end(); it++) {
        cout << it->first << " " << it->second << endl;
    }
}
```

## output

```cpp
1 10
2 20
3 30
4 40
5 50
```

## size()

*size() function returns the number of elements in the map.*

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    map<int, int> m;
    m[1] = 10;
    m[2] = 20;
    m[3] = 30;
    m[4] = 40;
    m[5] = 50;
    cout << m.size() << endl;
}
```

## output

```cpp
5
```

