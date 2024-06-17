# Data Collection

```milestone 3```

## Objectives

In this milestone objective is finding several real life simulations with known results. We will be satisfied with 1 - 2, if we didn't find much. The desired number should be 4 - 7.

## Criteria

- well documented
- from real life
- known results, 
- results could be presented in compatible format, so we would be able to compare them  
- populations could be transformed to Concordia actors
- settings could be transformed to Concordia GM settings


## Criteria updates

Having run several demo scene, I have come to this additional criteria, based on conclusions:

- Small setup: find simulation with 1-10 involved persons. Fields could include psychology, experimental theater, role-playing games
- For larger scale: the features of population that matters in simulation should be simple, and be based on simple decision, on simple reasoning on simple facts. We could sure expect that small increase in complexity would result in much increase of computations required with large scale simulations 

## Field of choices:

### Possible sources:

1. Small Group Dynamics Studies:
Bales' Interaction Process Analysis (IPA): This involves observing small groups (usually 5-7 participants) to study the interaction process and categorize behaviors into task-oriented and socio-emotional types. The structured nature of IPA makes it suitable for modeling with LLMs.
Link: [Interaction Process Analysis](https://en.wikipedia.org/wiki/Interaction_process_analysis)

2. Role-Playing Games (RPGs):
Small group RPGs provide structured yet flexible settings where participants adopt roles and make decisions based on predefined rules. Simulating these interactions using LLMs can be more straightforward as the decision space is well-defined.
Link: [RPG Research](https://www.rpgresearch.com/)

3. Economic Game Experiments:
Ultimatum Game: Involves two players where one proposes a division of a sum of money and the other accepts or rejects it. The simplicity and clear rules make it easier to model using LLMs.
Link: [Ultimatum Game](https://en.wikipedia.org/wiki/Ultimatum_game)

4. Experimental Theater:
Playback Theater: Involves actors enacting real-life stories told by the audience. This can be simulated with LLMs where actors respond to scripted prompts and audience reactions.
Link: [Playback Theater](https://en.wikipedia.org/wiki/Playback_Theatre)

5. Psychological Experiments on Decision Making:
Trolley Problem: Participants are asked to make moral decisions in a hypothetical scenario. This involves clear, discrete choices that can be modeled effectively by LLMs.
Link: [Trolley Problem](https://en.wikipedia.org/wiki/Trolley_problem)

6. Social Influence Studies:
Sherif's Autokinetic Effect Experiment: Studied how individuals' estimates of a moving light converged when in a group. The clear, quantifiable responses make it suitable for LLM simulation.
Link: [Autokinetic Effect Experiment](https://en.wikipedia.org/wiki/Autokinetic_effect)

7. Game Theory Experiments:
Prisoner's Dilemma: Involves two players making decisions to cooperate or defect, impacting each other's outcomes. The structured decision-making process is ideal for LLM-based simulations.
Link: [Prisoner's Dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma)

### Psychological / Social:

1. Stanford Prison Experiment:
Conducted in 1971 by Philip Zimbardo, this experiment involved 24 male university students who were assigned roles as either guards or prisoners in a mock prison environment. The study was intended to last two weeks but was terminated after six days due to the extreme psychological effects on participants. The experiment provides insights into the power of situational influences on behavior and social roles. [Source](https://www.apa.org/topics/forensics-law-public-safety/prison).

2. Stanford Marshmallow Experiment:
This series of experiments, conducted by Walter Mischel in the late 1960s and early 1970s, tested children's ability to delay gratification. Children were given a choice between one small reward provided immediately or two small rewards if they waited for a short period. The study involved various setups to understand the factors influencing self-control. [Source](https://en.wikipedia.org/wiki/Stanford_marshmallow_experiment).

3. Devah Pager's Employment Discrimination Studies:
Sociologists Devah Pager, Bruce Western, and Bart Bonikowski conducted field experiments to study discrimination in the low-wage job market. They used matched résumés with equivalent qualifications for white, black, and Latino job seekers to measure employer responses. This study provides insights into racial discrimination in employment. [Source](https://socialsci.libretexts.org/).

4. Robbers Cave Experiment:
Conducted by Muzafer Sherif in 1954, this experiment involved 22 boys at a summer camp divided into two groups to study intergroup conflict and cooperation. The study spanned three weeks and provided valuable data on how group identities and conflicts develop and can be resolved. Source.

5. Asch Conformity Experiments:
Solomon Asch's experiments in the 1950s involved small groups of participants who were asked to match line lengths. Unbeknownst to the actual participant, other members of the group were confederates instructed to give incorrect answers. The study explored the extent to which social pressure from a majority group could influence a person to conform. Source.

6. Milgram Experiment:
Stanley Milgram's study on obedience involved participants being instructed to administer electric shocks to another person (an actor) when incorrect answers were given to questions. This experiment aimed to understand obedience to authority figures and was conducted with a small number of participants in each session. Source.

7. Bystander Apathy Experiment:
Inspired by the murder of Kitty Genovese, this series of experiments by John Darley and Bibb Latané examined how the presence of others affects an individual's likelihood of helping someone in distress. These experiments involved small groups of participants and revealed the "bystander effect." Source.

8. Hawthorne Studies:
These experiments were conducted at the Hawthorne Works factory in the 1920s and 1930s to study how different working conditions affected worker productivity. Although the setup involved larger groups, specific experiments within the study focused on smaller groups and individual productivity. Source.

9. Festinger's Cognitive Dissonance Experiment:
Leon Festinger's experiment in the 1950s involved participants performing boring tasks and then being paid either $1 or $20 to tell a subsequent participant that the tasks were interesting. The study examined how cognitive dissonance (conflict between actions and beliefs) influenced attitudes. Source.

10. Little Albert Experiment:
Conducted by John B. Watson and Rosalie Rayner in 1920, this experiment involved conditioning a young child to fear a white rat by pairing the sight of the rat with a loud noise. This study provided insights into classical conditioning and emotional responses. Source.

## Fits

### 1. **Stanford Prison Experiment:**
Conducted in 1971 by Philip Zimbardo, this experiment involved 24 male university students who were assigned roles as either guards or prisoners in a mock prison environment. The study was intended to last two weeks but was terminated after six days due to the extreme psychological effects on participants. The experiment provides insights into the power of situational influences on behavior and social roles. [Source](https://www.apa.org/topics/forensics-law-public-safety/prison).

**Notes and consideration**: I believe we fill see different results here. Such effect, lead to termination of this experiment are more connected to feeling and emotional feedback. And our primary approach is to model LLM based on conscious decisions and evaluations. And so it will be good to try to input this experiment, trying to minimize bias, and see what we will observe. 

Experiment hold in [LLM_run](../4_llm_run) milestone.

2. 