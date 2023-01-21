# pairs
pairs in stl can be used to store pairs of values.
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
 pair<int, int> p = make_pair(10, 20);
 cout<<p.first<<" "<<p.second<<endl;
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
 pair<pair<int, int>, int> p = make_pair(make_pair(10, 20), 30);
 cout<<p.first.first<<" "<<p.first.second<<" "<<p.second<<endl;
}
```
## output
```cpp
10 20 30
```
## pair of vectors
```cpp
pair<vector<int>, vector<int>> p;
```
## example
```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
 vector<int> v1 = {1, 2, 3};
 vector<int> v2 = {4, 5, 6};
 pair<vector<int>, vector<int>> p = make_pair(v1, v2);
 for(int i = 0; i < p.first.size(); i++) {
  cout<<p.first[i]<<" ";
 }
 cout<<endl;
 for(int i = 0; i < p.second.size(); i++) {
  cout<<p.second[i]<<" ";
 }
 cout<<endl;
}
```
## output
```cpp
1 2 3
4 5 6
```
## pair of arrays
```cpp
pair<int[], int[]> p;
```
## example
```cpp

#include<bits/stdc++.h>
using namespace std;
int main() {
 int arr1[] = {1, 2, 3};
 int arr2[] = {4, 5, 6};
 pair<int[], int[]> p = make_pair(arr1, arr2);
 for(int i = 0; i < 3; i++) {
  cout<<p.first[i]<<" ";
 }
 cout<<endl;
 for(int i = 0; i < 3; i++) {
  cout<<p.second[i]<<" ";
 }
 cout<<endl;
}
``` 
## output
```cpp
1 2 3
4 5 6
```
