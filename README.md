# Actor Life Cycle Task

---

## Introduction

For this project, I was tasked with the creation of a simple C++ Actor Class in Unreal Engine, and to have it log a message from three different life cycle functions. To do this I simply created an actor that logs when it is constructed, when play begins, and every tick.  In order to simplify the process of the creation of this task, I used the previous task that I had done as a base, and added UE_LOG() to the Actors C++ file.

*Figure 1: Unreal Engine's Log showing messages sent.*
![An image of the log in unreal engine](./README%20Assets/log.png "")  

---

## Implementation

For this project I first used created a C++ class and a Header class for the C++ class to inherit from.

To begin with, I created an Actor C++ Class in Unreal, I then moved to Visual Studio by opening the solution file in order to edit the class.

I then opened MyClass.cpp and added this code within the constructor, AMyClass::AMyClass() in order to be sent in the log on the class's construction.

```
	UE_LOG(LogTemp, Warning, TEXT("Constructor"));
```

I then added this code within Begin Play function.

```
	UE_LOG(LogTemp, Warning, TEXT("Begin Play"));
```
I then added this code within the Tick function.
```
	UE_LOG(LogTemp, Warning, TEXT("Ticking"));
```


I then built the class and moved back to Unreal to check. When I pressed play in Unreal, the log successfully displayed the messages.

*Figure 3: An image of the log in unreal engine*
![An image of the log in unreal engine](./README%20Assets/log.png "")  

---

## Outcome

The final result of this has a C++ Actor Class that causes logs to appear when constructed, when the game begins play, and when it begins ticking.This meets the requirements of the task as I have successfully created an Actor that logs 3 different functions in Unreal Engine.

---

## Bibliography

Unreal Engine CPP Quick Start | Unreal Engine 5.7 Documentation | Epic Developer Community (s.d.) At: https://dev.epicgames.com/documentation/unreal-engine/unreal-engine-cpp-quick-start (Accessed  15/04/2026).
Verhoeff, S. (2026) Setting up Unreal Engine for C++ Development in 2026. At: https://medium.com/@sophia.verhoeff/setting-up-unreal-engine-for-c-development-in-2026-fcd56cd26392 (Accessed  15/04/2026).

## AI Usage Declaration

Copilot was used for the purposes of IntelliSense to assist with coding.
