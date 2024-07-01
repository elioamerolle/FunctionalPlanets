# Planetary System Simulator

The goal of this project is to give a very naive and fun way to see how planets might interact with each other in two dimensions. The simulation also assumes inelastic collisions where the moment to planets touch they become one.

## How To Run

In order to run this project it is heavily recommended to have conda installed. This will greatly simplify the instillation process. If you have conda run the following commands 

```sh
conda create -n "testEnv"
conda activate testEnv
```

Next you can run a shell script that installs all the necessary dependencies. This shell script will check if you have conda, pip and pip3 in that order and will attempt to install the necessary dependencies using the system available. If you have conda the environment used to develop the project is copied into the empty conda environment (testEnv) you have made

```sh
sh install.sh
```

*Note: If you do not have conda the shell script will not install python for you and install an arbitrary version of pygame*

The script installs python version 3.9.15 along with pygame version 2.1.2. Here pygame is used for the rendering of the various shapes to illustrate the actual simulation. 

Once the installation process is complete you can run the program with the command 

```sh
python Central.py
```

## Documentation of Code

The following code contains contains 3 classes that allow the program to run.

* `Arrow`: Inside of the Vector.py file, is responsible for the vectors associated with forces and velocity.

* `Planet`: This class contains the data for a hypothetical planet including mass and so forth as well as a rendering function that draws a circle and a function that considers the effect of gravity on the planet.

* `Funcs`: Many useful project specific functions are kept here. They generally deal with linear algebra, collision processing, and rendering.

