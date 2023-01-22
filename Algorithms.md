## sort

```cpp
sort(variable_name.begin(), variable_name.end());
```

#### example

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

#### output

```cpp
10 20 30
```

## reverse

```cpp
reverse(variable_name.begin(), variable_name.end());
```

#### example

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

#### output

```cpp
30 20 10
```

## find

```cpp
find(variable_name.begin(), variable_name.end(), value);
```

#### example

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

#### output

```cpp
found
```

## binary search

```cpp
binary_search(variable_name.begin(), variable_name.end(), value);
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    if(binary_search(v.begin(), v.end(), 20)) {
        cout<< "found" << endl;
    }
    else {
        cout<< "not found" << endl;
    }
}
```

#### output

```cpp
found
```

## lower bound

*lower_bound returns the first element which is not less than the given value if value is present otherwise it returns first element which is just greater than value*

```cpp
lower_bound(variable_name.begin(), variable_name.end(), value);
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    auto it = lower_bound(v.begin(), v.end(), 20);
    cout<< *it << endl;
}
```

#### output

```cpp
20
```

## upper bound

*upper_bound returns the first element which is greater than the given value irrespective of whether value is present*

```cpp

upper_bound(variable_name.begin(), variable_name.end(), value);
```

#### example

```cpp

#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    auto it = upper_bound(v.begin(), v.end(), 20);
    cout<< *it << endl;
}
```

#### output

```cpp
30
```



## max element

```cpp
*max_element(variable_name.begin(), variable_name.end());
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout<< *max_element(v.begin(), v.end()) << endl;
}
```

#### output

```cpp
30
```

## min element

```cpp
*min_element(variable_name.begin(), variable_name.end());
```

#### example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    vector<int> v = {10, 20, 30};
    cout<< *min_element(v.begin(), v.end()) << endl;
}
```

#### output

```cpp
10
```