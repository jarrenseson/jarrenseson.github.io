---
layout: project
type: project
image: img/8422225.png
title: "File Organizer"
date: 2024
published: true
labels:
  - Python
  - Scripting
summary: "I developed a Python program that arranges files based on their file extension"
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

As a computer science student, I found myself downloading many files, causing a state of disarray on my desktop. As such, I developed a Python automation script, that allowed me to simply run a line of code and arrange files by file extensions.

Here is some code that illustrates how we read values from the line sensors:

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
