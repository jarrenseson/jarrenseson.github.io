---
layout: project
type: project
image: /img/download.jpg
title: "ICS212: Bank Database Application"
date: 2024
published: true
labels:
  - C++
summary: "Simple banking application that allowed the user to add 'records' to a linked list, implemented by myself."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

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

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
