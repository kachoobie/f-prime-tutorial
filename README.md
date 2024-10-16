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

The setup here is quite similar to that on the official F' community Hello World page. I've added any notes I have about the process for clarity.

### Install fprime-bootstrap

```pip3 install fprime-bootstrap```

### Create a new fprime project

Try instantiating your project with command

```fprime-bootstrap project```

If this works for you, congratulations! Unfortunately for me, I couldn't for the life of me get this command to work. A workaround to this is to simply start your virtual environment immedately:

```python3 -m venv fprime-venv```
```. fprime-venv/bin/activate```

When the virtual environments in running, then run command

```fprime-bootstrap project```

You will be prompted to name your project, so do this.  

The command to create a F' project didn't work for me initially. I first had to add it as an environmental path.