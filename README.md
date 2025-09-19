# Movie Tracker

## Overview
This Python program helps users manage a personal movie watchlist.  
It allows you to:
- Update a list of unwatched movies
- Interactively mark movies as watched
- View statistics about your movie list
- Simulate saving watched movies

The program uses *modular design* and applies several *software design principles* to keep the code clean, readable, and easy to maintain.
---

## Software Design Principles

*Single Responsibility Principle (SRP):*  
The Single Responsibility Principle means that each object focuses on a specific task(s).  
In this program, each function does one job — for example, update_movies() only updates the movie list, and save_watched_movies() only handles saving.

*Encapsulation:*  
Encapsulation means keeping an object’s data and the methods that work on that data together, and controlling access to that data so it can’t be changed in unexpected ways.  
Here, each function manages its own data internally and doesn’t expose unnecessary details to other parts of the program.

*DRY (Don’t Repeat Yourself):*  
The DRY principle means avoiding duplicate code by reusing methods or functions, so changes only need to be made in one place.  
In this program, input handling and list updates follow similar patterns — these could be improved by creating reusable helper functions.

*Open/Closed Principle:*  
The Open/Closed Principle means code should be open to adding new features but closed to changing existing code.  
For example, you could add a movie rating feature or genre filtering without rewriting the core logic of tracking watched movies.

*Separation of Concerns:*  
Separation of Concerns means dividing a program into distinct sections, where each section handles a specific type of work.  
In this program, functions that update data (update_movies()) are separate from those that display or interact with the user (set_watched_movies()).

*Informations*  
Information Expert means giving a task to the part of the program that already has the information needed to do it.  
In this program, show_stats() has access to the movie list, so it’s the best place to calculate and display statistics.

*High Cohesion:*  
High Cohesion means keeping related tasks and data together in the same part of the program.  
Each function in this program is focused and self-contained, and the main flow runs all steps in a clear, logical order.

---

## How to Run
1. Install Python 3.x
2. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/movie-tracker.git
