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