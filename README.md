The ALX Project - The Maze Game
 

![img](https://github.com/user-attachments/assets/dcb8a934-0908-49e2-b659-d1ecebed30a5)


The goal of this Maze Game Project is to create a 3D game using the raycasting technique. Raycasting is a rendering technique used in computer graphics to simulate a 3D environment in a 2D space. I have always been fascinated and curious as to how games are made and how they are developed. Once this opportunity presented itself to develop a maze game using SDL2, C++ and the raycasting technique, I invested maximum time ensuring that I get a good grasp of what I needed to do to make this a reality. This project is to be implemented on Ubuntu 14.04 LTS using the gcc compiler and the SDL2 and SDL2_image library for graphics and input.

After the installation of SDL2, the test below was carried out to verify that SDL2 has been correctly installed:


#include <SDL2/SDL.h>
int main(int argc, char* argv[]) {
    if (SDL_Init(SDL_INIT_VIDEO) != 0) {
        printf("SDL initialization failed: %s\n", SDL_GetError());
        return 1;
    }

    SDL_Window* window = SDL_CreateWindow("SDL2 Test", SDL_WINDOWPOS_CENTERED, SDL_WINDOWPOS_CENTERED, 800, 600, 0);
    if (!window) {
        printf("Window creation failed: %s\n", SDL_GetError());
        return 1;
    }

    SDL_Delay(3000);

    SDL_DestroyWindow(window);
    SDL_Quit();

    return 0;
}

The Project Requirement
All functions in the code must be commented.
To promote consistency, all functions must be maximum 40 lines long (one statement per line) and maximum 80 columns long.
All codes must fit the Holberton School coding style.
All codes must be well documented in respect to the Holberton School documentation format
The entire repository is checked using Betty.
The Project Context
On the map in the maze game, the player can move in all four directions using keys W, A, S, and D.

The player can navigate through the maze, making left or right turns as desired.

If the player encounters a wall, they are unable to proceed unless they alter their direction.

The player has the capability to move in multiple directions and simultaneously rotate.

Installation
Clone this repository:

git clone https://github.com/majok31/Alx-maze-project.git

The Project Controls
W: Move forward.

S: Move backward.

A: Rotate left.

D: Rotate right.

Mouse movement left/right: Adjust your view to the left or right.

M: Disable the map display. Clicking won't show the 2D map.

N: Enable the map display. The 2D map will become visible once more if it was hidden.

The Project Directories
headers

All the header files are in here.

images

This contains all image files.

maps

This will be used by the program to output the map layout using the data map files

src

All the source code files written in C are in this folder.

tests

This folder contains the SDL2 test file.

Contributions
Begin by examining the source files located within the "src" directory and the header files in the "header" directory.

Duplicate the repository and establish a new branch using the following command: $ git checkout https://github.com/majok31/Alx-maze-project -b [name_of_new_branch].

Introduce a new feature, resolve any existing bugs, or undertake code refactoring as needed.

If applicable, create or revise test cases to ensure the changes are properly validated.

If necessary, update the README.md file to reflect any modifications.

Finally, initiate a Pull Request, providing a comprehensive description of the alterations made.

The Project Inspiration
The Maze Game Project is a game directly inspired by Wolfenstein3D, which was developed in 1992. For this project, a game engine was not required.

Author

Peter Ruot Tot

Github

The 3D Maze Game Project Demo(click 👇)
https://www.youtube.com/watch?v=7BfGxbB_suc

The 3D Maze Project
