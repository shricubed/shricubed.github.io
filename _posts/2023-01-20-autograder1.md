---
title: "CMSC388J Autograders"
categories:
  - Blog
tags:
  - Post Formats
  - coding
---

For this semester of CMSC388J, the Python and Flask class I teach, I'm writing autograders to speed up project grading. This is a simple one for the first Flask project, which requires students to code up a small website using the Pokemon API: https://github.com/shricubed/sample-python-pytest-autograder/blob/master/EXECUTION-FILES/run_tests.py. This is a fork of UCLA's autograder that was integrated with Pytest, and I added tests that access different routes on the website and checks whether they are set up correctly. I picked Pytest over the unittest module due to the fact that it is part of the class curriculum, and so is easier to integrate with more complex projects.

The PokeClient library has functions to access the API, and the ones used here are ```get_pokemon_list()```, which returns a list of all Pokemon names, ```get_pokemon_info()```, which returns a dictionary with information about a specific Pokemon, and ```get_pokemon_with_ability()```, which returns all Pokemon with the specified ability.
