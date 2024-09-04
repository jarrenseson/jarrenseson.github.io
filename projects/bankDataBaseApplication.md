---
layout: project
type: project
image: img/download.jpg
title: "ICS 212: Bank Database Application"
date: 2024
published: true
labels:
  - C++
summary: "Simple banking application that allowed the user to add 'records' to a linked list, implemented by myself."
---

This application was developed by me in my program structure class. I implemented the linked list data structure into C++. It allowed users to search, add, and delete records of bank users. Through developing this project, I gained insight into dynamic memory allocation, pointers, and interactions between UI and backend. 

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

[GitHub](https://github.com/jarrenseson/ICS-212-Bank-Database-Application.git)
