
![pymmo](https://github.com/luisoutomaior/pymmo/blob/main/pymmo.png?raw=true)



[![License: GPL-3.0](https://img.shields.io/badge/License-GPL%203.0-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)





**_PyMMO_** is a Python framework/template of a MMO game built using **_PyGame_** on top of Python's built-in **_socket_** module. This template implements a simple MMORPG with baked in features such as:
- **In-game chat bubbles** functionality;
- **Action battle system** with server-side processing functionality;
- Run on **cloud**, **locally** in your machine, or **anywhere in-between** due to the use of sockets.
- **Multithreaded client handling** on the server side
- **Minimal and easy to use** and only requires PyGame as a dependency

## Preview:
![pymmo_anim](https://user-images.githubusercontent.com/5900245/118595424-48c0aa80-b768-11eb-874f-af1c4893413f.gif)

## Requirements
- PyGame 2.0+

## Usage

### Running the PyMMO server
For all commands below you must be situated in the root folder of this repository.

In one terminal, run server via:
```sh
python server.py
```

### Running the PyMMO client template 
In another terminal, run the following to open a client, i.e. the game: 

```sh
python client.py
````

A game window will open and spawn two entities: a player object, which is your controllable character and comes in magenta; and an enemy object, which you can interact with. Both are added to the server. The names of all entities are shown alongside their health point bars.

### Open multiple clients for multiplayer functionality

Open an additional terminal, and run in it the following command to open a new client instance:
```sh
python client.py
````


Adjust network settings by changing IP and port values in macros.py according to your needs.

### In-game commands:
- **Move** your character via up/right/left/down keyboard arrows. 
- **Attack** an enemy or another player by pressing space. This will damage the entity you are overlapping with, and it can damage both "enemy" and "player" entities. When HP bar reaches zero, the entity is killed and removed from the server. 
- **Chat** in-game by pressing any lowercase letter to write text to the in-game chat floatting bubble. Press enter to publish the text bubble you entered to all other players in the scene.


