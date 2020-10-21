# Cpp-kpoints
```c++
#include <vector>
#include <string>
#include <iostream>
using namespace std;
int main(int argc, char** argv) {
    std::vector<int> vec;
    for (int i = 0; i < 100; i++)    
        vec.push_back(i);
    cout << "10:" << vec[10] << endl;
    cout << "size:" << vec.size() << endl;
    cout << "*************************" << endl;
    vector<int>::iterator it = vec.begin() + 10;
    vec.erase(it);
    cout << "10:" << vec[10] << endl;
    cout << "size:" << vec.size() << endl;
    while (!vec.empty()) {
        vec.erase(vec.end() - 1);
        cout << "size:" << vec.size() << endl;
        }*/
    string s = "hello world!";
    const string* cp = &s;
    cout << cp << "\n" << *cp << endl;
    return 0;
    vector<int> vec;
    for (int i = 0; i < 10; i++) {
        vec.push_back(i);
    }
    for (auto i : vec) {
        cout << i << endl;
    }
    for (auto &i : vec) {
        i *= 2;
        cout << i << endl;
    }
    return 0;
    int a1 = 21;
    int a2 = 21;
    int a3 = 21;
    int* const p1 = &a1;
    const int* p2 = &a2;
    int const* p3 = &a3;
    if ((*p1)+=1) {
        cout << 'p1' << *p1 << endl;
    }
    else {
        cout << 'p1' << *p1 << endl;
    }
   if (++(*p2)) {
        cout << 'p2:'<< *p2 << endl;
    }
    else {
        cout << 'p2:'<< *p2 << endl;
    }*/
    if ((*p3)+=1) {
        cout << 'p3' << *p3 << endl;
    }
    else {
        cout << 'p3' << *p3 << endl;
    }
    return 0;
}
```
