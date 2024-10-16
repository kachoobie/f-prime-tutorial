# F' Walkthrough (for Mac Users)

## Terminology

**Component** - An encapsulated system of code... sort of like single responsibility in OOD principles  
**Port** - Communication interface between components. The only way components can transmit information between each other  
**Command** - An ability of the component; an action a component can execute  
**Event** - Actions that a component has performed. If the command is an object, the event is an instance  
**Telemetry Channel** - Things the provide the state of a component. Ex. an altitude component can report a rocket's altitude and set intervals in the telemetry channel  
**Deployment** - A F' project build resulting in an executable  
**Topology** - Network of components connected by ports 


## Setup

I ran into a few problems while trying to complete the Hello World tutorial on the F' community page on MacOS. This mostly had to do with my fprime-bootstrap installation directory not being in my path.


### Install fprime-bootstrap

```pip3 install fprime-bootstrap```

If your installation location is not already in PATH, pip should throw a warning saying so. It will also give you the installation path.

To add the installation location to PATH, open .zprofile and add a new line:

```export PATH="<install_path>:$PATH"```

### Create new fprime project

Instantiate your project using command

```fprime-bootstrap project```

A prompt should appear asking for a project name, which should be filled out accordingly.


### Activate the virtual environment

cd into the project directory.

```cd MyProject```

Then, start the virtual environment:

```. fprime-venv/bin/activate```

To deactivate the virtual envrionment, simply use command ```deactivate``` in the command line while the virtual environemnt is running.


### Build and generate project

Run the following commands:

```
fprime-util generate
fprime-util build
```