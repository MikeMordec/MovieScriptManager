MovieScriptManager

MovieScriptManager is a Python-based system designed for managing movie scripts. It allows for flexible scene swapping, director assignments, and keyword-based searches within the script. This project demonstrates basic object-oriented programming concepts and string manipulation in Python.
Table of Contents

    Features
    Installation
    Usage
    Example
    Contributing
    License

Features

    Scene Swapping: Dynamically swap scenes in a movie script based on specified indices.
    Script Timings: Automatically generates timing for each scene in the script.
    Director Management: Assign different directors to different scenes.
    Keyword Search: Search the movie script for specific keywords and find related scenes.
    User Interaction: Allows users to input a keyword and get results for matching scenes.

Installation

To use this project, you need to have Python installed. Follow these steps to set up the project:

    Clone the repository:

    bash

git clone https://github.com/yourusername/MovieScriptManager.git

Navigate to the project directory:

bash

cd MovieScriptManager

Run the script:

bash

    python movie_script_manager.py

Usage

Here’s how you can use MovieScriptManager:

    The script initializes with a predefined list of movie scenes, their corresponding timings, and director assignments.
    If you specify scene swaps, the system will reorder scenes and their metadata accordingly.
    You can search the script for keywords like "enemy", "gadgets", and "mission". The system will return scenes where the keyword appears.

Example Usage

bash

$ python movie_script_manager.py
Michael Mordec, 6/28/22, Lab 8, CSC 242:
a class object has been constructed

• Bob opening teaser sequence (0)
• Sue subplot: enemy gets away with briefcase in hot air balloon (7)
...

please enter a keyword to search the movie sequences

1) enemy
2) gadgets
3) mission
----------------
Enter your choice: 1
[keyword(s) found]
in scene sequence number 2
"subplot: enemy gets away with briefcase in hot air balloon"

Flipping Scenes

The script allows you to swap two scenes based on the specified indices. For example:

python

flips = [(8, 9)]  # This swaps scene 9 and 10

Example Code

Here's a snippet from the project that showcases scene swapping:

python

for flip in self.flips:
    temp = self.script[flip[0]]
    self.script[flip[0]] = self.script[flip[1]]
    self.script[flip[1]] = temp

Contributing

Contributions are welcome! Please follow these steps if you want to contribute:

    Fork the repository.
    Create a new feature branch:

    bash

git checkout -b feature/AmazingFeature

Commit your changes:

bash

git commit -m 'Add some amazing feature'

Push to the branch:

bash

git push origin feature/AmazingFeature

Open a pull request.
