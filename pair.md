# pairs
*pairs in stl can be used to store pairs of values. pairs are used to store two values of different data types.*
## declaration
```cpp
pair<data_type1, data_type2> variable_name;
```
## initialization
```cpp
pair<data_type1, data_type2> variable_name = make_pair(value1, value2);
```
#### or
```cpp
pair<data_type1, data_type2> variable_name(value1, value2);
```

#### or
```cpp
pair<data_type1, data_type2> variable_name = {value1, value2};
```

## accessing elements
```cpp
variable_name.first;
variable_name.second;
```
## example
```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
 pair<int, int> p = {10, 20};
 cout<< p.first << " " << p.second << endl;
}
```
## output
```cpp
10 20
```
## pair of pairs
```cpp
pair<pair<int, int>, int> p;
```
## example
```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
 pair<pair<int, int>, int> p = {{10, 20}, 30};
 cout<< p.first.first << " " << p.first.second << " " << p.second << endl;
}
```
## output
```cpp
10 20 30
```
## array of pairs
```cpp
pair<int, int> p[];
```
## example
```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
    pair<int, int> p[] = {{1, 2}, {3, 12}, {10, 13}};
    for (int i = 0; i < 3; i++) {
        cout << p[i].first << " " << p[i].second << "\n";
    }
}
```
## output
```cpp
1 2
3 12
10 13
```