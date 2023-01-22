# Vectors

*vector in cpp is a dynamic array with the ability to resize itself automatically when an element is inserted or deleted, with their storage being handled automatically by the container.*

## declaration

```cpp
vector<data_type> variable_name;
```

## initialization

```cpp
vector<data_type> variable_name = {value1, value2, value3, ...};
```

#### or

```cpp
vector<data_type> variable_name(value1, value2, value3, ...);
```

#### or

### push_back()

*push_back() function adds a new element at the end of the vector, after its current last element.*

### emplace_back()

*emplace_back() function is used to insert a new element into the vector container, the new element is added to the end of the vector.*


```cpp
vector<data_type> variable_name;
variable_name.push_back(value1);
variable_name.push_back(value2);
variable_name.push_back(value3);
...
```
#### or 

```cpp
vector<data_type> variable_name;
variable_name.emplace_back(value1);
variable_name.emplace_back(value2);
variable_name.emplace_back(value3);
...
```

#### or

```cpp
vector<data_type> variable_name(size);
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v(5);
    for (int i = 0; i < v.size(); i++) {
        cout << v[i] << " ";
    }
}
```

#### output

```cpp
0 0 0 0 0
```



#### or

```cpp
vector<data_type> variable_name(size, value);
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v(3, 10);
    for (int i = 0; i < v.size(); i++) {
        cout << v[i] << " ";
    }
}
```

#### output

```cpp
10 10 10
```

#### or

### copy constructor

```cpp
vector<data_type> variable_name(vector_name);
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v1 = {10, 20, 30};
    vector<int> v2(v1);
    for (int i = 0; i < v2.size(); i++) {
        cout << v2[i] << " ";
    }
}
```

#### output

```cpp
10 20 30
```

## Accessing elements

```cpp
variable_name[index];
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout << v[0] << " " << v[1] << " " << v[2] << endl;
}
```

#### output

```cpp
10 20 30
```

## Iterating

### Index-based iteration

```cpp
for(int i = 0; i < variable_name.size(); i++) {
    cout<< variable_name[i] << " ";
}
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    for (int i = 0; i < v.size(); i++) {
        cout << v[i] << " ";
    }
}
```

#### output

```cpp
10 20 30
```

#### or

### For-each loop

```cpp
for(auto i : variable_name) {
    cout<< i << " ";
}
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    for (auto i : v) {
        cout << i << " ";
    }
}
```

#### output

```cpp
10 20 30
```

### iterator based iteration

```cpp
for(auto i = variable_name.begin(); i != variable_name.end(); i++) {
    cout<< *i << " ";
}
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    for (auto i = v.begin(); i != v.end(); i++) {
        cout << *i << " ";
    }
}
```

#### output

```cpp
10 20 30
```

## 2D vector

```cpp
vector<vector<int>> variable_name;
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<vector<int>> v = {{10, 20, 30}, {40, 50, 60}};
    for (auto i : v) {
        for (auto j : i) {
            cout << j << " ";
        }
        cout << endl;
    }
}
```

#### output

```cpp
10 20 30
40 50 60
```

## vector of pairs

```cpp
vector<pair<int, int>> variable_name;
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<pair<int, int>> v = {{10, 20}, {30, 40}};
    for (auto i : v) {
        cout << i.first << " " << i.second << endl;
    }
}
```

#### output

```cpp
10 20
30 40
```

## vector of strings

```cpp
vector<string> variable_name;
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<string> v = {"abc", "def", "ghi"};
    for (auto i : v) {
        cout << i << endl;
    }
}
```

#### output

```cpp
abc
def
ghi
```


