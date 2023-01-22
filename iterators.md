# Vector Iterators

*vector iterators in cpp are used to iterate over the vector. It is used to access the elements of the vector.*

## declaration

```cpp
vector<data_type>::iterator variable_name;
```

## begin()

*begin() function returns an iterator pointing to the first element of the vector.*

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {1, 2, 3, 4, 5};
    vector<int>::iterator it;
    it = v.begin();
    cout<< *it << endl;
}
```

## output

```cpp
1
```

## end()

*end() function returns an iterator pointing to the position after the last element of the vector.*

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {1, 2, 3, 4, 5};
    vector<int>::iterator it;
    it = v.end();
    cout<< *(it - 1) << endl;
}
```

## output

```cpp
5
```

## rbegin()

*rbegin() function returns a reverse iterator pointing to the last element of the vector.*


## rend()

*rend() function returns a reverse iterator pointing to the position before the first element of the vector.*


## iterator using iterators and for loop


## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {1, 2, 3, 4, 5};
    vector<int>::iterator it;
    for (it = v.begin(); it != v.end(); it++) {
        cout << *it << " ";
    }
}
```

## output

```cpp
1 2 3 4 5
```

## size

*size() function returns the number of elements in the vector.*

```cpp
variable_name.size();
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout << v.size() << endl;
}
```

#### output

```cpp
3
```

## inserting elements

```cpp
variable_name.insert(variable_name.begin() + index, value);
```

#### example

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

#### output

```cpp
10 15 20 30
```

### inserting multiple elements

```cpp
variable_name.insert(variable_name.begin() + index, size, value);
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    v.insert(v.begin() + 1, 2, 15);
    for (auto i : v) {
        cout << i << " ";
    }
}
```

#### output

```cpp
10 15 15 20 30
```

### inserting elements from another vector

```cpp
variable_name.insert(variable_name.begin() + index, variable_name.begin() + index, variable_name.begin() + index);
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v1 = {10, 20, 30};
    vector<int> v2 = {15, 25};
    v1.insert(v1.begin() + 1, v2.begin(), v2.end());
    for (auto i : v1) {
        cout << i << " ";
    }
}
```

#### output

```cpp
10 15 25 20 30
```

## deleting elements

```cpp
variable_name.erase(variable_name.begin() + index);
```

#### example

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

#### output

```cpp
10 30
```

### deleting multiple elements

```cpp
variable_name.erase(variable_name.begin() + index, variable_name.begin() + index);
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30, 40, 50};
    v.erase(v.begin() + 1, v.begin() + 3);
    for (auto i : v) {
        cout << i << " ";
    }
}
```

#### output

```cpp
10 40 50
```

## clearing the vector

*clear() clears the vector, i.e. it removes all the elements from the vector.*

```cpp
variable_name.clear();
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    v.clear();
    cout<< v.size() << endl;
}
```

#### output

```cpp
0
```

## empty

*empty() returns true if the vector is empty, otherwise it returns false.*

```cpp
variable_name.empty();
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout<< v.empty() << endl;
}
```

#### output

```cpp
0
```