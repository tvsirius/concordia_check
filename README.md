# Concordia_Check

Welcome to **Concordia_Check** Data Science project. This is a capstone project for the ELO part of the [MIT Emerging Talent 2023](https://emergingtalent.mit.edu/) Program

## Project description

*Can we really rely on LLMs (via Concordia) to simulate human beings?*

This project is based on [Concordia](https://github.com/google-deepmind/concordia) - a library for using LLMs to facilitate constructing and working with Generative Agent-Based Models (GABM), which can apply common sense to situations, act “reasonably,” recall common semantic knowledge, and communicate both within the simulation and to researchers viewing it from the outside.

Concordia allows the construction of language-mediated simulations of physically or digitally grounded environments and was designed to support a wide array of applications in scientific research and for evaluating the performance of real digital services by simulating users and/or generating synthetic data. This library may offer additional insights for using it not only for social simulations. We can imagine possible intersections with scenic art, psychology, science fiction, and many more. But first, the more important question comes to mind.

Concordia's general approach is to model living beings using LLMs and simulate virtual space inhabited by these "LLM-powered beings". One of the main proposed applications is social modeling, simulation, and predicting behavioral patterns of populations.

Let's find out if we can really rely on LLMs to simulate humans. How accurate could the results of such simulations be?

It should be possible to find some real social simulations conducted on populations of medium size. We will look for simulations of this kind that can be transformed into the Concordia virtual settings. And we will run this simulation in Concordia. Check if we need any fine-tuning. See what we get and compare it to the known results of the simulation we choose.

And I believe this is the way we will find answers to our question.


## Repository structure and navigation

The repository is organized in folders that corresponds to milestones. 
This project have started 2024 March. All documents are live documents now. 


## Milestones:

### [1 Problem Identification](1_problem_identification)

This milestone will have a clearly stated project idea, goals, constraints, research questions as deliverables.
[Read more...](1_problem_identification).

### [2 Concordia Demo Scene](2_concordia_demo_scene)

In this milestone we are exploring Concordia and running several demo simulations. [Read more...](2_concordia_demo_scene)

**Milestone 2 conclusions:**

- Local LLM deployment, like Llama 3. Need step, that will allow for experimentation of large scale. Comparison of simulation results with local vs OpenAI LLM could be considered. 
- This concept of **Chain Of Thought** should be well understood for further steps. 
- An experiment with 1-10 actors should be preferable options for the start.

### [3 Data Collection](3_data_collection)

In this milestone we will find several real life documented simulations, that could be scripted into Concordia settings. [Read more...](3_data_collection)

### [4 LLM Simulation run](4_llm_run)

In this milestone we will start our run of simulations. Conclusions, optimizations abd observations based on outcome. [Read more...](4_llm_run)

### [5 Analysis](5_analysis)

We performed an analysis of our simulation results. [Read more...](5_analysis/README.md)

## Conclusions

The results of our simulations demonstrate that while LLMs hold considerable promise in modeling human behavior, their effectiveness is highly dependent on the specific settings and the programming of the agents. The Ultimatum Game and Stanford Prison Experiment simulations showcased the ability of LLMs to generate coherent and contextually appropriate responses, reflecting basic psychological traits and stress responses. However, these simulations also highlighted limitations in strategic adaptability and emotional depth, indicating that current LLM implementations do not fully capture the complexities of human decision-making and variability in emotional responses. This suggests that while LLMs can simulate human behavior to a significant extent, there is still substantial work needed to enhance their accuracy and reliability.

Our findings underline the critical role of the simulation settings and the programming of agents in achieving realistic human behavior modeling. We do not yet have a universal agent capable of fully replicating human behavior across all scenarios. However, by fine-tuning the simulation parameters and incorporating principles from behavioral economics, as well as allowing agents to learn and adapt from interactions, we can approach a high level of likelihood in specific scenarios. Ongoing research and development in this field are crucial for advancing the capabilities of LLMs in social simulations, moving us closer to creating agents that can accurately model human behavior under varied and complex conditions.

## Next Steps

Coming soon...

## Links

[Generative agent-based modeling with actions grounded in physical, social, or digital space using Concordia](<resources/Generative agent-based modeling using Concordia.pdf>)

[Concordia repository](https://github.com/google-deepmind/concordia)

[Ragdoll-studio](https://ragdoll-studio.vercel.app/dolls#) 

[Llama 3](https://huggingface.co/meta-llama/Meta-Llama-3-8B)

[Llama.cpp - LLM quantization (running LLMs with limited amount of video memory)](https://github.com/ggerganov/llama.cpp)

[AI Town: Create a AI Virtual World 100% Local using Llama 3](https://www.youtube.com/watch?v=gjV4KIY5nqI)

## Similar/alike project

[AI Town hf](https://huggingface.co/spaces/radames/ai-town)

[AI Town MIT](https://github.com/a16z-infra/ai-town)


## Author

[Denys Savytskyi](https://github.com/tvsirius) / [LinkedIn](https://www.linkedin.com/in/denys-savytskyi-19b58777/)



