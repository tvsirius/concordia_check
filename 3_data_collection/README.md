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

## Selected simulations

### 1. **Ultimatum Game** 

The Ultimatum Game is a well-known experiment in economic psychology that explores decision-making and fairness. In this game, one participant (the proposer) is given a sum of money and must offer a portion of it to another participant (the responder). The responder can either accept or reject the offer. If the offer is rejected, both participants receive nothing. This game has been extensively studied, providing a wealth of documented results for comparison. [Wiki.](https://en.wikipedia.org/wiki/Ultimatum_game)

The Ultimatum Game has been extensively researched, providing ample documented results:

Typical Findings:
    Proposers often offer around 40-50% of the total sum.
    Offers below 20-30% are frequently rejected.
    Cultural differences can influence the outcomes, with some societies accepting lower offers more frequently than others.

Experiment hold in [Ultimatum Game](<../4_llm_run/Ultimatum Game>)

### 2. **Stanford Prison Experiment:**
Conducted in 1971 by Philip Zimbardo, this experiment involved 24 male university students who were assigned roles as either guards or prisoners in a mock prison environment. The study was intended to last two weeks but was terminated after six days due to the extreme psychological effects on participants. The experiment provides insights into the power of situational influences on behavior and social roles. [Source](https://www.apa.org/topics/forensics-law-public-safety/prison).

**Prior thesis**: I believe we will see different results here. Such effect, lead to termination of this experiment are more connected to feeling and emotional feedback. And our primary approach is to model LLM based on conscious decisions and evaluations. And so it will be good to try to input this experiment, trying to minimize bias, and see what we will observe. 

Experiment hold in [LLM_run/Stanford Prison Experiment](<../4_llm_run/Stanford Prison Experiment>).


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

### Role-playing / Game theory:

1. **The Prisoner’s Dilemma**:
   - **Description**: A scenario in game theory where two individuals may choose to cooperate or betray each other.
   - **Roles**: 2 players as prisoners.

2. **The Ultimatum Game**:
   - **Description**: A game where one player proposes a division of resources and the other can accept or reject it.
   - **Roles**: 2 players.

3. **The Dictator Game**:
   - **Description**: One player determines the division of resources without the input of the other.
   - **Roles**: 2 players.

4. **Sherif’s Autokinetic Effect Experiment**:
   - **Description**: Participants judge the movement of a light in a dark room, eventually conforming to a group norm.
   - **Roles**: 4 participants.

5. **The Bystander Effect**:
   - **Description**: Observing how the presence of others affects the likelihood of helping someone in distress.
   - **Roles**: 1 person in distress, 3 bystanders.

6. **The Stroop Effect Experiment**:
   - **Description**: Participants are asked to name the color of the ink of words that are color names.
   - **Roles**: 4 participants.

7. **The Invisible Gorilla Experiment**:
   - **Description**: Participants are asked to watch a video and count basketball passes, often missing a person in a gorilla suit walking through.
   - **Roles**: 4 participants (observers).

8. **The Iowa Gambling Task**:
   - **Description**: A psychological task thought to simulate real-life decision making.
   - **Roles**: 4 participants.

9. **The Trust Game**:
   - **Description**: One player decides how much money to send to another, which gets multiplied, and the second player decides how much to return.
   - **Roles**: 2 players.

10. **The False Memory Experiment**:
    - **Description**: Participants are given lists of words and later tested to see if they recall words that were not on the list.
    - **Roles**: 4 participants.

11. **The Candle Problem**:
    - **Description**: Participants are asked to attach a candle to a wall so that it does not drip onto the table below.
    - **Roles**: 4 participants.

12. **The Monty Hall Problem**:
    - **Description**: A probability puzzle based on a game show scenario.
    - **Roles**: 1 host, 3 participants.

13. **The Marshmallow Test**:
    - **Description**: Children are given a choice between one small reward now or two small rewards later.
    - **Roles**: 4 children (simulated).

14. **The Clark Doll Experiment**:
    - **Description**: Children are asked to choose between dolls of different races, examining the effects of segregation.
    - **Roles**: 4 children.

15. **The Stanford Marshmallow Experiment**:
    - **Description**: Similar to the Marshmallow Test, focusing on delayed gratification.
    - **Roles**: 4 children (simulated).

16. **The Good Samaritan Experiment**:
    - **Description**: Observing whether people will help someone in distress based on time pressure.
    - **Roles**: 1 person in distress, 3 participants.

17. **The Halo Effect Experiment**:
    - **Description**: Observing how impressions of a person's characteristics affect judgments about unrelated traits.
    - **Roles**: 1 target person, 3 evaluators.

18. **The Pavlov’s Dog Experiment**:
    - **Description**: Classical conditioning with dogs and bells.
    - **Roles**: 1 dog (simulated), 1 experimenter, 2 assistants.

19. **The Harlow’s Monkey Experiment**:
    - **Description**: Studying attachment in monkeys with surrogate mothers.
    - **Roles**: 1 monkey (simulated), 1 experimenter, 2 assistants.

20. **The Visual Cliff Experiment**:
    - **Description**: Testing depth perception in infants by having them crawl towards their mothers across a glass surface that appears to drop off.
    - **Roles**: 1 child, 1 mother, 2 observers.
