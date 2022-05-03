# **VERY TO-DO README.**

## HelperFunctions.cpp
* Just a small collection of functions I _used_ to help me in my console programs _back when_ I started coding.
* Not tested, maybe not correct, efficiency is a joke, but it's the solution _I use_.
* You are mostly better off with some other solution, you have been **warned**.
* If you are new to programming, this _might be_ a nice mini project.
---
## How to include?
* Put this at the start of your code:
```c++
#include "HelperFunctions.h"
```
---

## List of functions:

### 1- `ReadFile()`

#### Description:
* Reads from file, given `path` and `vector<string> Inlines`.

#### Program example:
```c++
// In a function or main()
vector<string> container;
ReadFile(container, "in.txt");

// each line is in a separate index.
cout << container[0];
```
* You can also use absloute path if needed.
```c++
ReadFile(container, "D:\\3_Studies\\MyGithubFolder\\3_OtherVentures\\HelperFunctionsCPP\\in.txt");
```

---
### 2- `ReadFileSplit()` 
---
### 3- `ReadFileSplit()` 
---
### 4- `WriteFile()` 

#### Description:
* Writes to file, given `path` and `vector<string> Outlines`.

#### Program example:
```c++
// In a function or main()
vector<string> container;
string data = "This is a string that will be added to the file\nNotice that this will be in a separate line.";
container.push_back(data);

WriteFile(container, "out.txt");
```
* This function **Overwrites** the file in `path`.
---
### 6- `SplitString()` 

#### Description:
* Splits string based on given `delimiter`, *returns* `vector<string>`.

#### Program example:
```c++
// Why this example?
// Refrence: UVa 196 - Spreadsheet
// https://onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&page=show_problem&problem=132

string str = "=A4+B51+D6+CZ31";

vector<string> splitted_string;
SplitString(splitted_string, str, '+');

cout << splitted_string[0] << " ? " << splitted_string[2];
```
* I used this one a lot, but I am still skeptical of its efficieny and correctness.
---
### 7- `StringToInt()` 

#### Description:
* Takes string and returns int.

#### Program example:
```c++
string test = "123";
cout << StringToInt(test) << '\n';

// Allows wrong input:
test = "+123";
cout << StringToInt(test) << '\n';

test = "123+";
cout << StringToInt(test);
```
* Allows negative values.
* Input **has** to be entirely numbers.
---
### 8- `IntToString()` 
* Takes int and returns string.
```c++
int num = 123;
cout << IntToString(num) << '\n';

num = -123;
cout << IntToString(num);
```
* Deals with negative values.
* Float datatypes **are not** supported.
---
### 9- `PrintLineHashed()` 
* Prints string to console (stdout) with added hashes => `#`.
```c++
PrintLineHashed("Test");
```
---
### 11- `PrintMenu()`
* Prints vector contents numbered.
```c++
vector<string> MainMenu = {"Login", "Register", "Exit"};
PrintMenu(MainMenu, "Login Menu");
```
---
### 12- `PrintPairs()` 
* Prints contents of two vectors as a pair. `(vector1[0], vector2[0])`
```c++
vector<string> UserDetails = {"First name", "Last name", "Gender"};
vector<string> UserInfo = {"Mo", "Gomaa", "M"};
PrintPairs(UserDetails, UserInfo, "User Info");
```
---
### 13- `VerifyChoice()` 
---

## Q/A:

* `Q:` Why aren't you making most of the functions return the needed container (e.g. `vector<string>`), instead you are passing said containers as a refrence?
* `A:` Because I don't want `copy()` constructor to be initialized, more efficient.
* Q:
---
## To-be added:
* Improve Readme.md
* Add `Example Program output` to Readme.md
* Add option of Append to `WriteFile()`.
* Use **ONE** naming convention.
* Add ability to change delimiter in `PrintMenu()` and `PrintPairs()`, I believe '\t' would be better.
* ...
###### Salam (:
