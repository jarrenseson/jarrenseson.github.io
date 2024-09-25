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
{
  int main() {
    int x = 10;

    if (x > 5)
        printf("X is greater than 5\n");
        printf("This will always print!\n");

    return 0;
  }
}
~~~
Since C doesn't rely on indentation, but {} one may think that because of the indentation the print statements will only be executed if the codition x > 5. However, in reality the print statements are not dependent on the conditional statement.

## Easier for Collaboration

Another thing I like TypeScript over JavaScript is static typing. Many times in JavaScript I found an error that took me a long time to fix simply because I didn’t use an “= 0”. Also, being able to see what the type is in the code makes the readability of the code significantly better and more predictable. Becuase of this, static typing also makes collaboration with teammates significantly easier and also makes scaling projects easier. Another benefit is being able to catch errors at compile time, preventing bugs, such as attempting to access undefined variables or a mismatched type error.

## Interfaces

Lastly, I also like TypeScripts inclusion of interfaces. It really helps being able to have an outline of an object saved, just like other programming languages. Because it forces objects to have a defined structure, it also makes errors get caught at compile time as opposed to run time. Because it defines an objects structure, it also allows for easier code reusability. Also, it allows for extensibility, allowing for more complex structures. 

## TypeScript for Software Engineering?

As a whole, I think that TypeScript is a good language for web development, as it adds many useful features, that attempt to compensate for JavaScript's shortcomings. For example, static styping and type annotations, allowing for greater scalability. Also, because of its active community, there is much documentation and third party tools. However, I think that web application development is the only application for it. For other types of applications there are more more suitable languages for the tasks at hand.

