# Sets

*sets in cpp are containers that store unique elements following a specific order.*

## declaration

```cpp
set<data_type> variable_name;
```

## insert()

*insert() function is used to insert new elements in the set container, the new element is added to the set.*

## example

```cpp

#include<bits/stdc++.h>
using namespace std;
int main() {
    set<int> s;
    s.insert(1);
    s.insert(2);
    s.insert(3);
    s.insert(4);
    s.insert(5);
    for(auto i : s) {
        cout<< i << " ";
    }
}

```

## output

```cpp
1 2 3 4 5
```

## erase()

*erase() function is used to remove elements from the set container, the element is removed from the set.*

## example

```cpp

#include<bits/stdc++.h>
using namespace std;
int main() {
    set<int> s;
    s.insert(1);
    s.insert(2);
    s.insert(3);
    s.insert(4);
    s.insert(5);
    s.erase(3);
    for(auto i : s) {
        cout<< i << " ";
    }
}

```

## output

```cpp
1 2 4 5
```

## pop()

*pop() function is used to remove the last element from the set container, the element is removed from the set.*

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    set<int> s;
    s.insert(1);
    s.insert(2);
    s.insert(3);
    s.insert(4);
    s.insert(5);
    s.pop();
    for(auto i : s) {
        cout<< i << " ";
    }
}

```

## output

```cpp
1 2 3 4
```

## count()

*count() function is used to count the number of elements with a specific key in the set container.*

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    set<int> s;
    s.insert(1);
    s.insert(2);
    s.insert(3);
    s.insert(4);
    s.insert(5);
    cout<< s.count(3) << endl;
}

```

## output

```cpp
1
```

## find()

*find() function is used to find the position of the element in the set container.*

## example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    set<int> s;
    s.insert(1);
    s.insert(2);
    s.insert(3);
    s.insert(4);
    s.insert(5);
    auto it = s.find(3);
    cout<< *it << endl;
}

```

## output

```cpp
3
```