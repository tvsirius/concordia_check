# Concordia Demo Scene

```milestone 2```

# About Concordia

[Article on Concordia](2312.03664.pdf) and a [Concordia GitHub repository](https://github.com/google-deepmind/concordia)

# Objective

The main objective of this milestone will be getting used to Concordia, and running a simple simulation. This step could be done in parallel to milestone 3 for better understanding if the simulations we choose fit.

# Demo Scene

## demo_01

I modified demo of "A day in Riverbend" that comes with Concordia and run it. The detailed README with inputs and outputs could be seen [here](demo01/README.md). Also the simulation produce a [HTML](http://tvsirius..github.io/concordia_check/2_concordia_demo_scene_docs/day_in_riverbend_output.html) with the history of the simulation day. 

Generally the results impress. I remembered [Westworld](https://en.wikipedia.org/wiki/Westworld_(TV_series)), as I was reading the logs, prompts and responses. Indeed there is a lot of complexity in the prompts, and these characters are really simple, but the story of their actions looks like real. After the simulation there is a option to communicate with the actors, conditioning on the history of the day. Despite "robot-like" correctness of their answers different actors answer like people with different character and personality. I tried to ask about the happiness score (0-100) in the morning and in the evening and get valid results. We could use this option, in different aspects, to get the evaluations, and metric scores for the simulations.
Of course in the results there could be seen hallucinations. In one conversation, that happened to be between two actors ended rough, on the question. Other thing is the feeling of "blind robots" who are diligently following their programs when you read the in the log about many of their actions. But this thing could be nether good nor bad, and could be like low level noise, that will have low impact on our experiments.

Another thing to consider is the price. This 1 day with 5 actors, and time quantization by 1 hour, from 8:00 to 20:00 (12 hours). I used 16K context window ```gpt-3.5-turbo-16k``` model. The simulation lasted 2186 API request, 900k context and 90k response tokens. It took 15 minutes and a **$2.72**.
This is a bit above my expectations. 

I will consider:
- smaller simulations 
- simpler actors
- larger quantization
- try to use other LLM, that could be deployed locally. Considering use of llama-3 8B, based on it's described functionality. This will require some effort. 

This also give some ideas about what kind of real simulations could fit in this project.
