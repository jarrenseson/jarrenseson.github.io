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

<img width="300px" class="rounced float-start pe-4" src="/img/codingStandardsPic.webp">

## Improved Readability

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
With the addition of the curly braces, the entire meaning of the code is changed. Now, the print statements will only be executed if x > 5. Simple things such as indentation can completely change the meaning of a piece of code, however this may vary from language to language. Python for example, relys on indentation instead of {}. Therefore, it is also important to consider the language a software is being developed in when coming up with coding standards.

## Decreased Errors
Coding standards often enforecs practice that help to fix common coding mistakes. By maintaining the coding standards we can ensure that common bugs that arise due to the lack of coding standards does not happen. For example, the coding standard of type safety, would help to reduce type-related errors. On a larger scale project, a type-related error could cause the whole program to not work properly. Another example of a coding standard that would help to decrease errors is version control. If there is an error that is caused due to a lack of overhead of the development of previously developed code, a developer can "reload" that code and work from there. Having to redevelop code would be less than ideal, however it sometimes must be done. Lastly, 
another common coding standard is the avoidance of duplicate code. Avoiding duplicate code allows for easier maintainability and overall easier development

## Easier for Collaboration
Something many people seem to forget when talking about development of larger software projects is that most of the time they are developed in teams. As such, having consistent coding standards throughout the project become much more important. By having easier to read code it makes it easier for each individual devloper to be able to leave where another may have left off. It is also important that everyone working on the project all have the same consistent coding standards. If everyone were to have different coding standards, it would be impossible for larger teams to come together to develop anything. Also, if members were to leave the team and onboard new members, the new members would have an exponentially more difficult time trying to adapt to everyone's different coding standards, especially those of the members that left. If the departed members also had no documentation on their coding standards, it would be possible that all of their progress made may have been for nothing.