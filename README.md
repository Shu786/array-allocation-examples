PLS Assignment 
### 📂 `array_categories.cpp` (C++)

```cpp
#include <iostream>
#include <vector>
using namespace std;

int main() {
    // a) Fixed Stack Dynamic
    int fixedStack[5] = {1, 2, 3, 4, 5};

    // b) Stack Dynamic (size decided at runtime)
    int n;
    cout << "Enter size: ";
    cin >> n;
    int* stackDynamic = new int[n];

    // c) Fixed Heap Dynamic
    int* fixedHeap = new int[5];
    for (int i = 0; i < 5; i++) fixedHeap[i] = i * 2;

    // d) Heap Dynamic using vector
    vector<int> heapDynamic;
    heapDynamic.push_back(10);
    heapDynamic.push_back(20);

    // Output
    cout << "FixedStack[0]: " << fixedStack[0] << endl;
    cout << "StackDynamic[0]: " << stackDynamic[0] << endl;
    cout << "FixedHeap[0]: " << fixedHeap[0] << endl;
    cout << "HeapDynamic[0]: " << heapDynamic[0] << endl;

    delete[] stackDynamic;
    delete[] fixedHeap;
    return 0;
}
```

---

### 📂 `array_categories.py` (Python)

```python
# a) Fixed Stack Dynamic
fixed_stack = [1, 2, 3, 4, 5]

# b) Stack Dynamic
n = int(input("Enter size: "))
stack_dynamic = [0] * n

# c) Fixed Heap Dynamic
fixed_heap = [i * 2 for i in range(5)]

# d) Heap Dynamic
heap_dynamic = []
heap_dynamic.append(10)
heap_dynamic.append(20)

# Output
print("FixedStack[0]:", fixed_stack[0])
print("StackDynamic[0]:", stack_dynamic[0])
print("FixedHeap[0]:", fixed_heap[0])
print("HeapDynamic[0]:", heap_dynamic[0])
```

---



Languages used: C++ and Python
```

| Feature             | Java                               | JavaScript                      |
| ------------------- | ---------------------------------- | ------------------------------- |
| Fixed Stack Dynamic | Local fixed-size array             | Simulated via scoped array      |
| Stack Dynamic       | Runtime-sized array on heap        | Native dynamic array            |
| Fixed Heap Dynamic  | Fixed-size heap-allocated array    | Simulated fixed-structure array |
| Heap Dynamic        | `ArrayList` or dynamic collections | Native array (fully dynamic)    |

