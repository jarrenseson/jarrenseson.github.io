---
layout: essay
type: essay
title: "Design Patterns: The Mold to all Locks"
# All dates must be YYYY-MM-DD format!
date: 2024-12-5
published: true
labels:
  - Design Patterns
  - Software Engineering
---

*In a technical interview, the question "what are design patterns?" and "what design patterns have you used in your own code" may be asked. As aspiring computer science graduates, we should be able to answer this question.*

<img width="300px" class="rounced float-start pe-4" src="/img/design_patterns.png">

## The Mold to Unlock any Lock

Throughout the process of software design, software developers will inevitably run into many issues. We can think of these issues as a lock, blocking us from the desired sofware. Since many of these "locks" commonly occur, software developers can use a mold to eventually make a key that can open these "locks". This "mold" is what a design pattern is. The "mold" represents the best practices to follow in order to make a key to unlock these "locks". The main thing that design patterns aim to do is to guide developers to develop software that is efficient, maintainable, and scaleable. There are many different types of design patterns, each meant to help solve some sort of problem. For example, the Factory design pattern addresses the problem of creating an object of a certain type when the class is unknown or can chage. It addresses this problem by defining an interface for object creation and allowing its subclasses to determine what class to instantiate.

## My Journey With Design Patterns

 A project of mine that demonstrated my use of a design pattern, specifically the model-view-controller pattern is a web application jewelry store. This design pattern splits the application into 3 different parts. The first is the model, which handles data and logic. The second is the view, which handles the user interface. The third is the controller, which handles interactions between the user and the model or view accordingly. As a whole, using the model-view-controller helped to simplify a lot of things. The main parts of the application were able to be worked on mostly independently and rarely affected the other parts of the project. Because I used the moodel-view-controller design pattern I ended up with a clean, scaleable, and maintainable structure.