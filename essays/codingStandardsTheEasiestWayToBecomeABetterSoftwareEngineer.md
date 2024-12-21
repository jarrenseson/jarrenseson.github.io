---
layout: essay  
type: essay  
title: "Coding Standards: The Easiest Way to Become a Better Software Engineer"  
# All dates must be YYYY-MM-DD format!  
date: 2024-09-26  
published: true  
labels:  
  - Software Engineering  
  - Coding Standards  

---

*While coding standards are often viewed as menial and monotonous, they are a critical aspect of software engineering and something all good software engineers value.*

<img width="300px" class="rounded float-start pe-4" src="/img/codingStandardsPic.webp">

## Improved Readability  

One of the simplest reasons to adopt good coding standards is that they make code easier to read. The way code is formatted can drastically influence how we perceive what a piece of code will do versus what it actually does. Take this snippet of C code, for example:  

~~~c  
if (x > 5)  
  printf("X is greater than 5\n");  
  printf("This will always print!\n");  
~~~  

Since C doesn't rely on indentation but rather `{}` for code blocks, one might think that, because of the indentation, the print statements will only execute if the condition `x > 5` is true. However, in reality, the print statements are not dependent on the conditional statement. Here's what the code would look like with the implementation of good coding standards:  

~~~c  
if (x > 5) {  
  printf("X is greater than 5\n");  
  printf("This will always print!\n");  
}  
~~~  

With the addition of curly braces, the meaning of the code becomes clear: the print statements will only execute if `x > 5`. Simple formatting choices, such as indentation and proper use of braces, can completely change the meaning of code. However, this may vary between programming languages. Python, for instance, relies on indentation instead of `{}`. Therefore, it is essential to consider the language being used when establishing coding standards.

## Decreased Errors  

Coding standards often enforce practices that help prevent common coding mistakes. By adhering to these standards, we can ensure that bugs arising from poor coding habits are minimized. For instance, the coding standard of type safety helps reduce type-related errors. In large-scale projects, such errors could cause the entire program to malfunction.  

Another example is the use of version control as a standard. If errors arise due to changes in previously developed code, version control allows developers to revert to an earlier version and proceed from there. While redeveloping code is less than ideal, version control minimizes the need for such efforts.  

Finally, avoiding duplicate code is another common standard that improves maintainability and simplifies development overall. By eliminating redundant code, developers can focus on building scalable and efficient solutions.

## Easier Collaboration  

Many people overlook the fact that large software projects are often developed collaboratively in teams. As such, consistent coding standards throughout a project become essential. Readable, standardized code makes it easier for individual developers to pick up where others have left off.  

It is equally important for everyone on the team to follow the same coding standards. Without consistency, large teams would find it nearly impossible to work together effectively. Moreover, if team members leave and new ones join, onboarding becomes significantly more difficult if coding standards are inconsistent or undocumented. In cases where departing members fail to document their standards, the progress they made may become unusable, potentially setting the entire project back.
