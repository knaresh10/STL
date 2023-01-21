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

## push_back() and emplace_back()

*push_back() function adds a new element at the end of the vector, after its current last element.*

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

## example

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

## output

```cpp
0 0 0 0 0
```



#### or

```cpp
vector<data_type> variable_name(size, value);
```

## example

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

## output

```cpp
10 10 10
```



## accessing elements

```cpp
variable_name[index];
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout << v[0] << " " << v[1] << " " << v[2] << endl;
}
```

## output

```cpp
10 20 30
```

## iterating

```cpp
for(int i = 0; i < variable_name.size(); i++) {
    cout<< variable_name[i] << " ";
}
```

#### or

```cpp
for(auto i : variable_name) {
    cout<< i << " ";
}
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    for (int i = 0; i < v.size(); i++) {
        cout << v[i] << " ";
    }
    cout << endl;
    for (auto i : v) {
        cout << i << " ";
    }
    cout << endl;
}
```

## output

```cpp
10 20 30
10 20 30
```

## size

```cpp
variable_name.size();
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout << v.size() << endl;
}
```

## output

```cpp
3
```

## sorting

```cpp
sort(variable_name.begin(), variable_name.end());
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    sort(v.begin(), v.end());
    for (auto i : v) {
        cout << i << " ";
    }
}
```

## output

```cpp
10 20 30
```

## reverse

```cpp
reverse(variable_name.begin(), variable_name.end());
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    reverse(v.begin(), v.end());
    for (auto i : v) {
        cout << i << " ";
    }
}
```

## output

```cpp
30 20 10
```

## inserting elements

```cpp
variable_name.insert(variable_name.begin() + index, value);
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    v.insert(v.begin() + 1, 15);
    for (auto i : v) {
        cout << i << " ";
    }
}
```

## output

```cpp
10 15 20 30
```

## deleting elements

```cpp
variable_name.erase(variable_name.begin() + index);
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    v.erase(v.begin() + 1);
    for (auto i : v) {
        cout << i << " ";
    }
}
```

## output

```cpp
10 30
```

## deleting all elements

```cpp
variable_name.clear();
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    v.clear();
    cout<< v.size() << endl;
}
```

## output

```cpp
0
```

## searching

```cpp
find(variable_name.begin(), variable_name.end(), value);
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    auto it = find(v.begin(), v.end(), 20);
    if(it != v.end()) {
        cout<< "found" << endl;
    }
    else {
        cout<< "not found" << endl;
    }
}
```

## output

```cpp
found
```

## max element

```cpp
*max_element(variable_name.begin(), variable_name.end());
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout<< *max_element(v.begin(), v.end()) << endl;
}
```

## output

```cpp
30
```

## min element

```cpp
*min_element(variable_name.begin(), variable_name.end());
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout<< *min_element(v.begin(), v.end()) << endl;
}
```

## output

```cpp
10
```
