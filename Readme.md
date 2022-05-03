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
* Reads from file, given `path` and `vector<string> inlines`.
  
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
---
### 5- `AppendFile()` 
---
### 6- `SplitString()` 
---
### 7- `StringToInt()` 
---
### 8- `IntToString()` 
---
### 9- `PrintLineHashed()` 
---
### 10- `PrintDecorated()` 
---
### 11- `PrintMenu()` 
---
### 12- `PrintPairs()` 
---
### 13- `VerifyChoice()` 
---

## Q/A:

* `Q:` Why aren't you making most of the functions return the needed container (e.g. `vector<string>`), instead you are passing said containers as a refrence?
* `A:` Because I don't want `copy()` constructor to be initialized, more efficient.
* Q:
---
###### Salam (:
