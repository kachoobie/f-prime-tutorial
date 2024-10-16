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

I ran into a few problems while trying to complete the Hello World tutorial on the F' community page on MacOS. The following steps worked for me.

### Create your virtual environment

```
python3 -m venv fprime-venv
. fprime-venv/bin/activate
```

The first line creates a virtual environment repository and the second activates the virtual environment. To validate the virtual environment is active, ```(fprime-venv)``` should precede every new line in the command line. If the virtual environment is inactive, simply run ```. fprime-venv/bin/activate``` again. To terminate the virtual envionemnt, enter command ```deactivate``` in the command line.


### Install fprime-bootstrap

```pip3 install fprime-bootstrap```


### Create new fprime project

Instantiate your project using command

```fprime-bootstrap project```

A prompt should appear asking for a project name, which should be filled out accordingly.
