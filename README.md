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
#### Unreal Engine Store Assets: 
- Templates: First Person and Third Person (unused)
- Open World Demo Collection
- Military Style Mannequins

#### Models:
- https://sketchfab.com/3d-models/a-bloody-kitchen-knife-01d6d4906ed749329f37c4929a4846aa
- https://sketchfab.com/3d-models/abandoned-drugslab-indoor-fd612e2ea8e94d80ac3b8097eb2e5bbe#download
- https://sketchfab.com/3d-models/alchemy-lab-isometric2020challenge-8002f00110804fd393a5ccb7ade21da5
- https://sketchfab.com/3d-models/alchemy-stuff-6863824addaa4115aabf4455e9c6573f
- https://sketchfab.com/3d-models/alchemy-table-free-09e4710c5f7247c39202442a352023a5
- https://sketchfab.com/3d-models/alchemy-table-game-model-ecc545e35e7c4d5dba91f94b98ba95b5
- https://sketchfab.com/3d-models/skyrim-alchemy-table-71b2039d24d64cd0a48dbfe94f19c1b0
- https://sketchfab.com/3d-models/alembic-811618ea79ba4aac95d7f7312a2128ec
- https://sketchfab.com/3d-models/antique-book-small-4d9627d6370f45a5aa186263858a6a55
- https://sketchfab.com/3d-models/antique-leather-book-big-f62314240a0140a89e29119829aec000
- https://sketchfab.com/3d-models/antique-book-with-quill-and-key-6be47f12c73342ef9232e29f71e0fa76
- https://sketchfab.com/3d-models/asset-graveyard-the-darkest-red-d9e14354303147849d6ef59644436692
- https://sketchfab.com/3d-models/blood-altar-f810136b88474a6d8a9b3155c1471770
- https://sketchfab.com/3d-models/bloody-baseball-bat-with-nails-425e6efd8d81408fa63ff2c2962840d1
- https://sketchfab.com/3d-models/bloody-eyes-mask-f89de732abae4018986e0958cb52c793
- https://sketchfab.com/3d-models/corpse-f99e4aac71754d599f0a5d10ef791718
- https://sketchfab.com/3d-models/cart-corpse-the-darkest-red-ac2389d2b9224b9d9310a6dfc978a7cc
- https://sketchfab.com/3d-models/demon-zombie-monster-pbr-game-ready-d4a333c91cb54fcbb19f54354548efe4
- https://sketchfab.com/3d-models/doom-hell-knight--2ff3458809da4f3d867a9edfc3ee5f43
- https://sketchfab.com/3d-models/door-2738468b94d74c5f827e7e5df7be8359
- https://sketchfab.com/3d-models/flowercorpse-64e2932c26ef4f95ad22cbf497866ea4
- https://sketchfab.com/3d-models/gate-01-97ca5ddd1e3b4346a6d3659525dc9263
- https://sketchfab.com/3d-models/godless-goddess-twelve-moons-78e0c259642d4c298b36dbaabf0b31af
- https://sketchfab.com/3d-models/human-transmutation-circle-fullmetal-alchemist-4ad153e685f64e15a1d0453041b3248a
- https://sketchfab.com/3d-models/hut-8fb506cdbfb94c80b4e01954f2ec803e 
- https://sketchfab.com/3d-models/kukri-on-the-bloody-ground-3fbc7efb1b3c4b39a43b6170e6d8ed12
- https://sketchfab.com/3d-models/low-poly-covered-corpse-44bbd7a61aa347439e42f0f10f7fb1de
- https://sketchfab.com/3d-models/medieval-bookcase-86d0148ab525424ea3bdea13430d476e
- https://sketchfab.com/3d-models/mortar-0e9b6e96a047410a80c31adddddb2e11
- https://sketchfab.com/3d-models/murder-scene-cloth-body-2775896b55c54d21a82e4aa1d485ec15
- https://sketchfab.com/3d-models/mutant-soldier-72e56e2f79dc413eb409d7b05571dc27
- https://sketchfab.com/3d-models/mystical-creature-rahu-fh-e3f533e80f124611a6d97ec6af66b318
- https://sketchfab.com/3d-models/old-bloody-wrench-9cee36d438964e03855d9b59b2343260
- https://sketchfab.com/3d-models/old-car-post-apocaluptic-2d9974c64d74454e9b3d8107fc715ea9
- https://sketchfab.com/3d-models/remains-7663ab71893f44b2b6466db3c625b061
- https://sketchfab.com/3d-models/respected-greatshield-e3080da12b2e42c484fdb1eced6c1260
- https://sketchfab.com/3d-models/roof-1-bake-5202c58077844c9ea9578e829d3da969
- https://sketchfab.com/3d-models/room-door-animation-e85909e80635445b92fb80772af80c84
- https://sketchfab.com/3d-models/shabby-books-94ee482748744253b52b8e3d38fdfab2
- https://sketchfab.com/3d-models/skull-sculpture-two-ee29eec0ca904c0bb8f346a8183d85c5
- https://sketchfab.com/3d-models/skull-sculpture-two-ee29eec0ca904c0bb8f346a8183d85c5
- https://sketchfab.com/3d-models/st-andrews-church-south-huish-84e4d984e29c4c9ca9b2bde12e6032b4
- https://sketchfab.com/3d-models/transmutation-platform-0119f385ee334603ae491f89a8ca248f
- https://sketchfab.com/3d-models/warn-wardrobe-b3a99e956be64ab6958f7f5e1895f031
- https://sketchfab.com/3d-models/window-4e596e7530d749068fa0aba2902b63df
- https://sketchfab.com/3d-models/zack-the-meat-sack-walk-cycle-5c83999ae6be456aaaeccc628f248d12
- https://sketchfab.com/3d-models/zombie-the-burnt-263514e15f3c4ef792796399876ca8a8
- https://www.mixamo.com/#/?page=1&query=monster&type=Character
- https://www.mixamo.com/#/?page=3&query=idle&type=Motion%2CMotionPack
- https://www.mixamo.com/#/?page=1&query=run&type=Motion%2CMotionPack
- https://drive.google.com/file/d/1Xt84jo8cPFo7RGVG9DWSbfAJeMxn87yW/view
- https://sketchfab.com/3d-models/sergery-scene-02ab1cf4a25047e5950a63a6f3c1077d
- https://www.turbosquid.com/de/3d-models/free-tiffany-key-jewelry-3d-model/595623
- https://www.turbosquid.com/de/3d-models/nine-volt-battery-fbx-free/935328

#### Sounds:
- https://freesound.org/people/Tissman/sounds/530777/
- https://www.freesoundeffects.com/free-track/nmh-scream1-466424/
- https://freesound.org/people/ckvoiceover/sounds/401336/
- https://freesound.org/people/InspectorJ/sounds/416076/
- https://freesound.org/people/silversatyr/sounds/113364/
- https://freesound.org/people/the_yura/sounds/211527/
- https://freesound.org/people/jacobmathiassen/sounds/254869/
- https://freesound.org/people/gumballworld/sounds/386923/
- https://freesound.org/people/Topschool/sounds/404142/
- https://freesound.org/people/Thegamemakerqueen/sounds/472100/
- https://freesound.org/people/flex0rnaut/sounds/465911/
- https://freesound.org/people/InspectorJ/sounds/485009/
- https://freesound.org/people/InspectorJ/sounds/418262/
- https://freesound.org/people/mrjingles/sounds/17184/
- https://freesound.org/people/InspectorJ/sounds/347850/
- https://freesound.org/people/DRFX/sounds/441286/
- https://freesound.org/people/InspectorJ/sounds/413549/
- https://freesound.org/people/InspectorJ/sounds/370937/
- https://freesound.org/people/InspectorJ/sounds/412224/
- https://freesound.org/people/InspectorJ/sounds/413315/
- https://freesound.org/people/engreitz/sounds/79769/
- https://freesound.org/people/kintana24/sounds/478934/
- https://freesound.org/people/Kalibrk/sounds/433921/
- https://freesound.org/people/FunWithSound/sounds/381374/
- https://freesound.org/people/ryanconway/sounds/239585/
- https://freesound.org/people/soundguy528/sounds/272350/
- https://freesound.org/people/sound-master/sounds/57683/
- https://freesound.org/people/timtube/sounds/61033/
- https://freesound.org/people/onderwish/sounds/469141/
- https://freesound.org/people/InspectorJ/sounds/413150/
- https://freesound.org/people/TheSubber13/sounds/239900/
- https://freesound.org/people/LloydEvans09/sounds/321832/
- https://mixkit.co/free-sound-effects/monster/

#### Pictures:
- https://i.pinimg.com/originals/0f/55/0c/0f550c8c1af7fa7ef60f7130aac85eb1.jpg
- https://imed.guru/wp-content/uploads/2019/01/insomnia.jpg
- https://i.pinimg.com/564x/23/ae/a6/23aea6bccb038e372a03012de808d9ff.jpg

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
