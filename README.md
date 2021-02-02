<!--
*** Thanks for checking out this README Template. If you have a suggestion that would
*** make this better, please fork the repo and create a pull request or simply open
*** an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
-->





<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]



<br />
<p align="center">
  <a href="https://github.com/Silices/turbo-potatoes">
    <img src="images/logo.jpg" alt="Logo" width="200" height="200">
  </a>

  <h3 align="center">Just a Nightmare ?</h3>

  <p align="center">
    <br />
    <a href="https://github.com/Silices/turbo-potatoes"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Silices/turbo-potatoes">View Demo</a>
    ·
    <a href="https://github.com/Silices/turbo-potatoes/issues">Report Bug</a>
    ·
    <a href="https://github.com/Silices/turbo-potatoes/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Basic Idea](#basic-idea)
  * [Features](#features)
  * [Assets](#assets)
  * [Built With](#built-with)
* [Development Guidelines](#development-guidelines)
  * [Git Workflow](#git-workflow)
  * [Code Review](#code-review)
  * [Other Guidelines](#other-guidelines)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)
* [Acknowledgements](#acknowledgements)



<!-- ABOUT THE PROJECT -->
## About The Project
### Basic Idea
* Genre: 3D Horror
* Story: Suddenly, the player finds himself on an abandoned and enclosed terrain. The only visible exit needs a certain 4 digit code.
  As he walks around on the premises, he might find out that he isn't as alone as he thought to be.
  And once he mangaes to escape, was it all just a nightmare ?

### Features
* Player Character (nothing but a crosshair).
* Movement Bindings: WASD, arrow-keys + space for jump.
* Stamina system (Shift-key to run).
* Flashlight with limited energy. (F-key to activate and R-key to reload).
* Pick-up Batteries (with E-key), to reload the flashlight.
* Pick-up Keys and Code-parts (with E-key).
* Doors With KeyLock, can be opened with a key (with E-key), once unlocked they have an opening animation.
* Doors with Keypad, they have an interactible keypad. Aim with the crosshair and press E to enter a digit, once unlocked they have an opening animation.
* For every interactible (items, doors etc.), once in range, a widget shows up indicating what key to press and whether it can be opened or not (for the doors at least).
* For the Keypad door, there is an extra widget at the bottom left corner, which indicates the already collected code pieces.
* Red outline for interractible items once looked at.
* Main-, pause- and death- menu. Each with interractible buttons and the according functionality.
* Win Screen.
* Enemies that follow you around once in radius and sight, they follow you around and kill you once they get close enough. They have a kill animation, where they scream at you.
* 2 types of jump scares: 
  - Screamer: fullscreen-size picture gets added to the players viewport + scream sound.
  - MovingObject: once in radius, a humanoid mannequin runs away from the player + weird sound.
* Random Sounds: 28 different random sounds/music that get played, once the player hits the corresponding collider.
* Music: 
  - Background music
  - Player walk sounds (different sounds depending on the ground type, such as grass, stone and wood).
* UI: battery-life indicator, battery amount indicator, stamina bar.
* Big detailed map, with high resolution and lots of space to explore.
* Fun gameplay.



### Controlls
* Movement: WASD keys, Arrow keys
* Jump: Spacebar
* Run: Shift key
* Pause Menu: ESC key
* Interracting: E key
* Flashlight: F key for turning on/off + R key for reload

### Assets

### Built With

* [Unreal Engine](https://www.unrealengine.com/)
* Version: 4.26
* Template: First Person and Third Person (unused)

<!-- DEV GUIDELINES -->
## Development Guidelines

### Git Workflow

***Feature-Branch-Workflow***  
1. Before starting your work on a new feature, always pull the newest version of [main](https://github.com/Silices/turbo-potatoes/tree/main) branch.  
2. Create a new branch from main and give it a descriptive Name 
    * You can use your trello card id and name for this, which can be found in the card url (for example 12-decide-on-a-git-workflow)
3. You can now work on your feature, commit and push changes inside of your Feature Branch. Make sure to always choose **descriptive** commit messages.
4. Once you have pushed all your changes for the feature, create a pull request to main branch in GitHub and assign a team member for code review.
5. If your pull request has been approved, the pull request can be merged into main.
    * If you encounter merge conflicts, merge main branch into your feature branch **locally** and push the merge commit afterwards.

### Code Review 

This is a list of things you can look out for while doing code review:
* Does the code follow all naming conventions?
* Is the code too complex or can it be done simpler?
* Are all comments clear and helpful?
* Has the developer provided/updated documentation for their changes?
* Does the code function the way it is intended?
* Does the code follow our style guides?

### Other Guidelines

Always create your own scene if you want to test changes, the MainScene should be in a functioning state at all times.  
If you do make changes to a Scene you want to share, make sure to save your changes in unity before pushing to git.  

<!-- GETTING STARTED -->
## Getting Started


### Prerequisites

_Add prerequisites if required_

### Installation

_Add installation steps if required_

<!-- USAGE EXAMPLES -->
## Usage
[Documentation](https://example.com)

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/Silices/turbo-potatoes/issues) for a list of proposed features (and known issues).

<!-- CONTRIBUTING -->
## Contributing
* Bartholomäus Berresheim
* Kenneth Englisch
* Marie Lencer
<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- CONTACT -->
## Contact

Project Link: [https://github.com/Silices/turbo-potatoes](https://github.com/Silices/turbo-potatoes)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Silices/turbo-potatoes?style=flat-square
[contributors-url]: https://github.com/Silices/turbo-potatoes/graphs/contributors
[issues-shield]: https://img.shields.io/github/issues/Silices/turbo-potatoes?style=flat-square
[issues-url]: https://github.com/Silices/turbo-potatoes/issues
[license-shield]: https://img.shields.io/github/license/Silices/turbo-potatoes?style=flat-square
[license-url]: https://github.com/Silices/turbo-potatoes/blob/master/LICENSE
