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

## reverse iterator

```cpp
vector<data_type>::reverse_iterator variable_name;
```

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {1, 2, 3, 4, 5};
    vector<int>::reverse_iterator it;
    for (it = v.rbegin(); it != v.rend(); it++) {
        cout << *it << " ";
    }
}
```

## output

```cpp
5 4 3 2 1
```