# 🌟 C++ Strings Guide 🚀
----------------------------------------
## 📌 1. Including Required Libraries
```cpp
#include <iostream>
#include <string>
using namespace std;
```

## 📌 2. Declaring Strings
```cpp
//Remember beginers , because were using the namespace std we dont need to write the data type like std::string we can just say string :)
string str1 = "Hello";  // 🌟 Using double quotes
string str2("World");  // 🌟 Constructor method
string str3{'C', '+', '+'};  // 🌟 Character list
```

## 📌 3. Taking Input
```cpp
string name;
cout << "Enter your name: ";
cin >> name;  // 🔹 Takes first word only
g getline(cin, name);  // 🔹 Takes full line
```

## 📌 4. Concatenation
```cpp
string fullName = str1 + " " + str2;  // 🔗 Using '+' operator
str1.append(str2);  // 🔗 Using append()
```

## 📌 5. Accessing Characters
```cpp
char firstChar = str1[0];  // 🎯 Get first character
str1[0] = 'h';  // ✏️ Modify character
```

## 📌 6. String Length
```cpp
int len = str1.length();  // 📏 Get length
int size = str1.size();  // 📏 Alternative method
```

## 📌 7. Substrings
```cpp
string sub = str1.substr(0, 3);  // 🔎 Get first 3 characters
```

## 📌 8. Finding Substrings
```cpp
size_t pos = str1.find("llo");
if (pos != string::npos) {
    cout << "Found at index: " << pos << endl;
}
```

## 📌 9. Replacing Substrings
```cpp
str1.replace(0, 2, "Hi");  // ✨ Replace first 2 characters with "Hi"
```

## 📌 10. Erasing Characters
```cpp
str1.erase(1, 2);  // ❌ Remove 2 characters from index 1
```

## 📌 11. Inserting Characters
```cpp
str1.insert(1, "ey");  // 📝 Insert "ey" at index 1
```

## 📌 12. Comparing Strings
```cpp
if (str1 == str2) cout << "Equal";  // 🔄 Direct comparison
if (str1.compare(str2) == 0) cout << "Equal";  // 🔄 Using compare()
```

## 📌 13. Converting String to Integer & Vice Versa
```cpp
string numStr = "123";
int num = stoi(numStr);  // 🔢 Convert to integer
string strNum = to_string(num);  // 🔠 Convert to string
```

## 📌 14. Iterating Over a String
```cpp
for (char ch : str1) {
    cout << ch << " ";  // 🔄 Loop through each character
}
```

## 📌 15. Reversing a String
```cpp
reverse(str1.begin(), str1.end());  // 🔄 Reverse string
```

## 📌 16. Transforming to Uppercase/Lowercase
```cpp
for (char &ch : str1) ch = toupper(ch);  // 🔠 Convert to uppercase
for (char &ch : str2) ch = tolower(ch);  // 🔡 Convert to lowercase
```

## 📌 17. Checking if String is Empty
```cpp
if (str1.empty()) cout << "String is empty";  // 🚫 Check if empty
```

## 📌 18. Clearing a String
```cpp
str1.clear();  // 🧹 Clear string
```

## 📌 19. Using C-Style Strings
```cpp
char cstr[] = "Hello";
printf("%s", cstr);  // 🏗️ Print C-string
```

## 📌 20. Converting C++ String to C-String
```cpp
const char* cstr = str1.c_str();  // 🔗 Convert to C-string
```
