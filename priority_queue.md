# priority queues in cpp
*Priority queues are a type of container adapters, specifically designed such that the first element of the queue is the greatest of all elements in the queue and elements are in nonincreasing order*
### syntax for declaring priorty queues

***priority_queue<data_type> variable;***

>example
```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
	priority_queue<int> pq;
}

```
---
### push method to insert elements into the priority queue

***variable.push(element);***
 >example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
	priority_queue<int> pq;
	pq.push(13);
	pq.push(10);
	pq.push(12);
}

```
----
### pop method to remove the highest element of the priority queue

***variable.pop();***
 >example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
	priority_queue<int> pq;
	pq.push(13);
	pq.push(10);
	pq.push(12);
	pq.push(15);
	pq.pop();
}

```
----
### top method is used to see the highest element present in the priority queue

***data_type variable1 = variable.top();***
 >example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
	priority_queue<int> pq;
	pq.push(13);
	pq.push(10);
	pq.push(12);
	pq.push(15);
	pq.pop();

	int var = pq.top();
	cout << var;
}
```

## output:

>13
----
### to traverse the priority queue we use the following code

***while(!variable.empty()) {***
\
***cout << variable.top();***
\
***variable.pop();***
***}***
 >example

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
	priority_queue<int> pq;
	pq.push(13);
	pq.push(10);
	pq.push(12);

	while (!pq.empty()) {
		cout << pq.top() << " ";
		pq.pop();
	}
}
```

## output:

>13 12 10 
