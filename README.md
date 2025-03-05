# crowd-evacuation project

# Implementation Plan for Disaster Evacuation Path Planning using MARL

## Phase 1: Algorithm Selection and Improvement (1 month)

### Week 1-2:
- Build disaster evacuation scenarios in Unity.
- Research MATD3 and MA-SAC algorithms.
- Select the most suitable algorithm based on the application scenario.
  - [MATD3 Algorithm Details](https://docs.agilerl.com/en/latest/api/algorithms/matd3.html)
  - [MA-SAC Algorithm Details](https://github.com/puyuan1996/MARL)

### Week 3-4:
- Integrate the improved social force model into the selected MARL algorithm.
- Design the leader-follower model for global path planning.

## Phase 2: Model Implementation and Training (2 months)

### Week 5-8:
- Implement the leader-follower model in the MARL framework.
- Train the MARL model using the improved social force model and leader-follower strategy.
- Validate the model performance in various scenarios and adjust parameters.

### Week 9-12:
- Continuously train and refine the model.
- Perform initial performance testing and adjustments.

## Phase 3: Unity Simulation (1 months)

### Week 13-14:
- Implement the interface between Unity and the MARL algorithm.
  - [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents)
  - [Unity Reinforcement Learning Integration Guide](https://unity-technologies.github.io/ml-agents/Getting-Started/)
- Conduct initial simulation tests to ensure proper integration.

### Week 15-16:
- Conduct multiple simulation tests to record evacuation times and paths.
- Fine-tune the Unity simulation environment for accuracy and realism.

## Phase 4: Performance Comparison and Optimization (1 month)

### Week 17-21:
- Compare the MARL algorithm with baseline static path planning algorithms.
- Metrics for comparison:
  - Average evacuation time
  - Loss and reward trends during training
- Optimize the algorithm and model based on comparison results.
- Final validation of the optimized model in various scenarios.

## Deliverables:
- Detailed documentation of the MARL algorithm implementation and improvements.
- Unity simulation environment with integrated MARL algorithm.
- Comparative analysis report with evacuation times, loss, and reward comparisons.
- Final optimized model ready for deployment in disaster management scenarios.

## Feasibility Analysis

### Algorithm Feasibility
- **MATD3**: Combines Twin Delayed Deep Deterministic Policy Gradient (TD3) with multi-agent systems, suitable for tasks requiring high stability.
- **MA-SAC**: Combines Soft Actor-Critic (SAC) framework with multi-agent systems, suitable for continuous action space problems with good sample efficiency.

### Social Force Model and Leader-Follower Model
- The improved social force model can realistically simulate crowd behavior.
- The leader-follower model effectively implements global path planning by having leaders guide the rest of the crowd.

### Unity Simulation
- The Unity ML-Agents toolkit provides a rich interface and tools for reinforcement learning simulation and testing.
- Unity's simulation capabilities enable realistic disaster evacuation scenarios and testing.

### Comparison Methods
- **Evacuation Time**: Measure the average evacuation time under different algorithms.
- **Loss and Reward**: Compare the trends of loss and reward during training between the MARL algorithm and baseline algorithms.
## Relevant Resources and Tools
- [MATD3 Algorithm Details](https://docs.agilerl.com/en/latest/api/algorithms/matd3.html)
- [MA-SAC Algorithm Details](https://github.com/puyuan1996/MARL)
- [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents)
- [Unity Reinforcement Learning Integration Guide](https://unity-technologies.github.io/ml-agents/Getting-Started/)
- [Data-driven crowd evacuation](https://www.sciencedirect.com/science/article/pii/S0925231219311488)
- [Crowd evacuation path planning and simulation method](https://link.springer.com/article/10.1007/s10489-024-06074-w)
