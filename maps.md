# Maps

## Introduction

*maps in cpp are associative containers that store elements in a mapped fashion. Each element has a key value and a mapped value. No two mapped values can have same key values. stored in sorted manner*

## declaration

```cpp
map<data_type1, data_type2> variable_name;
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    map<int, int> m = {
        {1, 10},
        {2, 20},
        {3, 30},
        {4, 40},
        {5, 50}
    }
    for (auto it = m.begin(); it != m.end(); it++) {
        cout << it->first << " " << it->second << endl;
    }
}
```

#### output

```cpp
1 10
2 20
3 30
4 40
5 50
```

## inserting elements

```cpp
variable_name[key] = value;
```

#### example

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

#### output

```cpp
1 10
2 20
3 30
4 40
5 50
```

#### or

```cpp
variable_name.insert({key, value});
```

#### example

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
    m.insert({6, 60});
    for (auto it = m.begin(); it != m.end(); it++) {
        cout << it->first << " " << it->second << endl;
    }
}
```

#### output

```cpp
1 10
2 20
3 30
4 40
5 50
6 60
```

#### or 

## Iterate through map

```cpp
for (auto it = m.begin(); it != m.end(); it++) {
    cout << it->first << " " << it->second << endl;
}
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    map<int, int> m = {{1, 10}, {2, 20}, {3, 30}, {4, 40}, {5, 50}};
    for (auto it = m.begin(); it != m.end(); it++) {
        cout << it->first << " " << it->second << endl;
    }
}
```

## for each loop

```cpp
for (auto it : m) {
    cout << it.first << " " << it.second << endl;
}
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    map<int, int> m = {{1, 10}, {2, 20}, {3, 30}, {4, 40}, {5, 50}};
    for (auto it : m) {
        cout << it.first << " " << it.second << endl;
    }
}
```

#### output

```cpp
1 10
2 20
3 30
4 40
5 50
```

## size()

*size() function returns the number of elements in the map.*

#### example

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

#### output

```cpp
5
```

## find()

*find() function returns an iterator to the element if the element is found, else returns m.end()*

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    map<int, int> m = {{1, 10}, {2, 20}, {3, 30}, {4, 40}, {5, 50}};
    auto it = m.find(3);
    if (it != m.end()) {
        cout << it->first << " " << it->second << endl;
    }
}
```

#### output

```cpp
3 30
```

## erase()

*erase() function removes the element from the map.*

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    map<int, int> m = {{1, 10}, {2, 20}, {3, 30}, {4, 40}, {5, 50}};
    m.erase(3);
    for (auto it : m) {
        cout << it.first << " " << it.second << endl;
    }
}
```

#### output

```cpp
1 10
2 20
4 40
5 50
```