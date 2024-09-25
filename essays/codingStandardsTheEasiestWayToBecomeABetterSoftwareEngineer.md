---
layout: essay
type: essay
title: "Coding Standards: The Easiest Way to Become a Better Software Engineer"
# All dates must be YYYY-MM-DD format!
date: 2023-9-26
published: true
labels:
  - Software Engineering
  - Coding Standards
---

*While coding standards can often be viewed as menial and rather monotonous, they are an important aspect of software engineering and is something that all good software engineers value.*

## Easier to Understand Code

One of the simpler reasons to have good coding standards is that it makes it easier for code to be read. The way that code is formatted can drastically change what we think a piece of code will do vs what it actually does. Take this snippet of C code for example:
~~~
if (x > 5)
  printf("X is greater than 5\n");
  printf("This will always print!\n");
~~~
Since C doesn't rely on indentation, but {} one may think that because of the indentation the print statements will only be executed if the codition x > 5. However, in reality the print statements are not dependent on the conditional statement. Here is what the code would look like with the implementation of good coding standards: 
~~~
if (x > 5) {
  printf("X is greater than 5\n");
  printf("This will always print!\n");
}
~~~
With the addition of the curly braces, the entire meaning of the code is changed. Now, the print statements will only be executed if x > 5.

## Easier for Collaboration
Something many people seem to forget when talking about development of larger software projects is that most of the time they are developed in teams. As such, having consistent coding standards throughout the project become much more important. By having easier to read code it makes it easier for each individual devloper to be able to leave where another may have left off. It is also important that everyone working on the project all have the same consistent coding standards.