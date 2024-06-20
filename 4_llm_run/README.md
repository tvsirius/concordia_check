# LLM Simulation run

```milestone 4```

## Objectives

> Past objective: In this milestone we will explore and deploy local LLM, starting with Llama 3. Starting our first run of best simulation found. Optimizing approach to simulations. If possible we will compare one run using local LLM and OpenAI LLM. **This objective was postponed to the future development. Until now ChatGPT 3.5 or 4-omni (pros and cons considered) will satisfy our needs 

Algorithm for running simulations, from [data collection fits](../3_data_collection/README.md#fits): 

1. Settings the experiment into Concordia settings. Trying to minimize bias.
2. Run
3. Results observation
4. Interviewing participants
5. Was the settings ok? - If not goto p. 1, it yes - continue
6. Thought on the results

## 1. [Ultimatum Game](<Ultimatum Game>)

[Classical game](https://en.wikipedia.org/wiki/Ultimatum_game) that have been widely explored. I believe we should obtain results close to the typical findings: *Proposers often offer around 40-50% of the total sum. Offers below 20-30% are frequently rejected. Cultural differences can influence the outcomes, with some societies accepting lower offers more frequently than others.* [See more...](<Ultimatum Game>)

### Results:

The results from our Ultimatum Game simulation using df_results0 and df_results1 significantly deviated from expected human behavioral patterns in similar scenarios, revealing a lack of strategic depth and realistic decision-making in the agents. Uniform and universally accepted offers, regardless of fairness, suggest that the agents' algorithms lack the complexity necessary for realistic gameplay. To improve the simulation's fidelity, we recommend enhancing the agents' decision-making capabilities, integrating behavioral economics principles, introducing dynamic strategy adjustments based on previous interactions, and incorporating diverse cultural backgrounds. These refinements aim to better mimic human behavior, providing a more accurate and insightful tool for studying economic decision-making and social interactions.

## 2. [Stanford Prison Experiment](<Stanford Prison Experiment>)

Conducted in 1971 by Philip Zimbardo, this experiment involved 24 male university students who were assigned roles as either guards or prisoners in a mock prison environment. The study was intended to last two weeks but was terminated after six days due to the extreme psychological effects on participants. The experiment provides insights into the power of situational influences on behavior and social roles. [Source](https://www.apa.org/topics/forensics-law-public-safety/prison).

A big one. Original expectations did not prove, and there is much to consider. [See more...](<Stanford Prison Experiment>)

### Results:

We have run 1 day of Stanford Prison experiment

#### Well-being Change of players

| Player | Well-being Change (-10 .. 10) |
|--------|--------------------|
| **Guards** | |
| Mike   | 1  |
| John   | 2  |
| Alex   | -1 |
| Steve  | -2 |
| Kevin  | -3 |
| Paul   | 0  |
| **Prisoners** | |
| Ryan   | -1 |
| Sam    | -3 |
| Chris  | -7 |
| David  | -4 |
| Jack   | -8 |
| Adam   | 1  |

The Stanford Prison Experiment simulation using LLMs provided a detailed look into the potential of these models to replicate human behavior under controlled conditions. The LLMs successfully generated distinct psychological profiles and responses, demonstrating their capability to simulate human-like reactions within the experiment's structured environment. While the simulation portrayed realistic psychological states and behaviors, the accuracy of these models in capturing the full spectrum of human emotions and individual nuances was limited, highlighting the complexity of human psychology. Factors such as the roles, environment, and specific stressors of the experiment played significant roles in influencing the outcomes and the fidelity of the simulation. To enhance the accuracy and depth of such simulations, a hybrid approach that combines LLMs with real-time data inputs and expert human oversight is suggested. This could lead to more dynamic and nuanced social simulations, providing a richer understanding of human behaviors in complex scenarios.