# Boids-Simulation

This model simulates complex ecosystem dynamics within a three-dimensional environment using an extended Boids framework that includes predator-prey interactions and resource competition. The main objective is to explore how changes in behavior and environment settings affect population sustainability and energy dynamics among predators and prey.

## HOW IT WORKS

The model incorporates several agent behaviors: alignment, cohesion, and separation to simulate flocking dynamics. Predators hunt prey to gain energy, while prey consume environmental resources (leaves) to survive. Agents possess a finite amount of energy that depletes with activity, influencing their survival and reproductive capabilities. The environment includes spatial boundaries that agents must navigate, creating a more dynamic interaction space.

| Cohesion | Separation | Alignment |
| :------: | :--------: | :-------: |
| <img src="(https://github.com/selcukemiravci/Enhanced-Boids-Simulation/assets/53044008/d26c0148-9d4f-4011-b1ab-f5c8b2cdc4f6" height="200" /> | <img src="https://github.com/selcukemiravci/Enhanced-Boids-Simulation/assets/53044008/de164875-f4d5-4b03-9a89-721d2c306fc0" height="200" /> | <img src="https://github.com/selcukemiravci/Enhanced-Boids-Simulation/assets/53044008/a200d502-6db3-456e-a54a-1c75503ebd7f" height="200" /> |
**Note:** For a demonstration of the Minimized Vision effect, see the corresponding GIF:  
<img src="https://github.com/selcukemiravci/Enhanced-Boids-Simulation/assets/53044008/f38dd6e6-c023-4f3e-97bc-50c382952b33" height="200" />

## HOW TO USE IT

1. **Setup Button**: Initializes the simulation with the specified number of predators, prey, and environmental features.
2. **Go Button**: Starts the simulation, allowing the agents to move according to the defined rules.

**Sliders:**

- **Population**: Adjusts the number of prey at the start of the simulation.
- **Vision**: Sets the distance each agent can perceive its surroundings, affecting its interactions.
- **Population-Predator**: Determines the initial number of predators.
- **Minimum-Separation**: Defines the minimum distance agents try to maintain from each other.
- **Max-Align-Turn**: Controls the maximum angle agents can turn towards the average heading of their flockmates per tick.
- **Max-Cohere-Turn**: Sets the maximum turning angle towards the average position of nearby agents to maintain group cohesion.
- **Max-Separate-Turn**: Limits the maximum turning angle away from nearby agents to avoid collision.

**Switches:**
- **Unlimited-Energy?**: When turned on, agents do not deplete energy, removing the energy constraint from behavior.

**Monitors and Plots:**
- **Population Plot**: Tracks the number of predators and prey over time.
- **Energy Levels Plot**: Displays the change in energy levels for prey, predators, and the availability of leaves.

## THINGS TO NOTICE

Observe how the initial conditions set by the sliders affect the population dynamics. Notice how quickly energy levels change and how they correlate with population changes. Pay attention to how the  `Unlimited-Energy? ` switch impacts the survival and behavior of agents.

## THINGS TO TRY

- Maximize and the  `Vision ` slider while minimizing other parameters like  `Max-Align-Turn ` to see how enhanced perception affects the agents' ability to survive and form flocks. Then try the opposite.
- Experiment with different levels of `Minimum-Separation` to observe how crowd density affects collision rates and overall flock movement.
- For a comprehensive test run utilizing all parameters, toggle the `Unlimited-Energy?` switch on, set `Vision` and `Max-Align-Turn` to their maximum values, adjust `Minimum-Separation` and `Max-Cohere-Turn` to mid-levels, and keep `Max-Separate-Turn` on the lower end. This setup will allow you to observe how high perception and alignment capabilities impact agent behavior when energy constraints are removed, while still maintaining a moderate degree of cohesion and minimal separation.

## EXTENDING THE MODEL

- Add age attributes to agents to introduce generational changes and life cycles.
- Implement varying energy gain from leaves depending on their type or nutritional value.
- Include seasonal changes that affect resource availability and agent behavior.

## NETLOGO FEATURES

This model utilizes NetLogo's 3D capabilities to simulate agent movement and interaction in a spatially complex environment. Custom sliders and switches are used to manipulate variables in real-time, allowing dynamic exploration of ecological theories.

## RELATED MODELS

- **[Wolf Sheep Predation](https://ccl.northwestern.edu/netlogo/models/WolfSheepPredation)**: Similar predator-prey dynamics but in a simpler ecological model.
- **[Flocking](https://www.netlogoweb.org/launch#http://ccl.northwestern.edu/netlogo/models/models/Sample%20Models/Biology/Flocking.nlogo)**: Basic behaviors of flock formation and movement dynamics.

## CREDITS AND REFERENCES

I would like to extend my deepest gratitude to Dr. Omar Addam for attending the guest lecture and presenting his inspiring project on Boids simulation, which significantly influenced the development of my own project. I am also profoundly thankful to Professor Christian Jacob for his invaluable discussions and insights regarding this project and for his exceptional lectures, which have greatly enriched my understanding of the subject.

- [NetLogo Flocking Model](https://www.netlogoweb.org/launch#http://ccl.northwestern.edu/netlogo/models/models/Sample%20Models/Biology/Flocking.nlogo)
- [NetLogo 3D Tree Model](https://ccl.northwestern.edu/netlogo/models/TreeSimple3D)
- [NetLogo Wolf Sheep Predation Model](https://ccl.northwestern.edu/netlogo/models/WolfSheepPredation)
- [Omar Addam's Boids Simulation on GitHub](https://github.com/omar-addam/Boids-Simulation)
- [Wikipedia: Boids](https://en.wikipedia.org/wiki/Boids)



