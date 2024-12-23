---
layout: essay
type: essay
title: "UI Frameworks: The Highest ROI skill?"
# All dates must be YYYY-MM-DD format!
date: 2023-10-10
published: false
labels:
  - UI Frameworks
  - Bootstrap 5
---

*Despite UI frameworks being complicated and having many niche attributes, they are an important skill to learn that will overall improve and simplify user interactions.*

<img width="300px" class="rounded float-start pe-4" src="/img/bootstrap5.jpg">

## The Challenging Part
It is true that UI frameworks are not the easiest to work with, and learning to use them to their full potential can take a while. There are many classes and other components that a developer must become familiar with. It may seem as if using pure HTML and CSS is more straightforward. However, attempting to achieve responsiveness, consistency, and compatibility across browsers is much harder with only HTML and CSS.

## Save Time
One of the biggest benefits of using UI frameworks is that it helps developers to save time. Instead of having to develop components each time a developer wishes to add a new element, a UI framework provides developers with pre-designed components such as buttons, navigation bars, grids, forms, etc. For example, Bootstrap 5 provides developers with classes that aid in the simplification of the navigation bar. Here is what a navigation bar would look like without Bootstrap 5:
~~~
  <style>
    body {
      font-family: Arial, sans-serif;
    }
    .navbar {
      background-color: #f8f9fa;
      padding: 1rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .navbar-brand {
      font-weight: bold;
      font-size: 1.5rem;
    }
    .navbar ul {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
      gap: 1rem;
    }
    .navbar li {
      display: inline;
    }
    .navbar a {
      text-decoration: none;
      color: black;
      padding: 0.5rem 1rem;
    }
    .navbar a:hover {
      background-color: #e2e6ea;
      border-radius: 0.25rem;
    }

    @media (max-width: 768px) {
      .navbar ul {
        display: none;
        flex-direction: column;
        gap: 0;
      }
      .navbar.active ul {
        display: flex;
      }
      .navbar-toggler {
        display: inline-block;
        cursor: pointer;
        background-color: #ccc;
        padding: 0.5rem;
        border-radius: 0.25rem;
      }
    }
  </style>
</head>
<body>

  <nav class="navbar">
    <div class="navbar-brand">Brand</div>
    <div class="navbar-toggler" onclick="toggleMenu()">☰</div>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <script>
    function toggleMenu() {
      const navbar = document.querySelector('.navbar');
      navbar.classList.toggle('active');
    }
  </script>
</body>
</html>
~~~
and here is what it would like with it:
~~~
<body>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Brand</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Services</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
~~~
As you can see, the navigation bar with Bootstrap 5 is a lot more concise and simpler than the one without. Bootstrap 5 allows for responsive elements without the hassle of implementing them.

## Consistency
UI frameworks also allow for easier consistency among web applications because they have a standardized design system. This can be especially helpful for larger projects, where multiple people are working on an application. By having a consistent design throughout the entirety of the web application, it appears more professional. Also, at least for Bootstrap, it was developed with a mobile-first approach, which means its first prerogative is responsive design. This means that web applications will function well and appear relatively the same on any screen size. Doing this with pure HTML and CSS would take considerably more work than using Bootstrap.

## Community Support/Documentation
These UI frameworks are typically designed by larger groups of developers and have strong communities behind them. As such, there is extensive documentation available. Common bugs that occur are documented, and their solutions are noted. This makes debugging much simpler. If you were to run into a bug while only using pure HTML and CSS, there is a chance that you will not be able to find a solution to the issue, making it much more time-consuming to fix.



