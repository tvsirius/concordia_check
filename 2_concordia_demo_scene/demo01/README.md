# demo_01: A Day in Riverbend

Here is detailed description of the demo_01

## About

This demo comes with Concordia. I have made slight changes, and run it with my OpenAI key.
Now this is a demo for 1 day of Riverbend where 5 people live. We are given the initial setting, their characters and objectives, with a element of randomness, that impact their behavior. All detail could be seems [here](https://github.com/google-deepmind/concordia/tree/main/examples/village).

## Notes

Simulation require 16K 'gpt-3.5-turbo-16k' model. The RUN part (the simulation itself) run about 15 minutes. The API usage for a simulation of 1 day costs $2.7.

## Input

Riverband have a small town with this settings:
```
shared_memories = [
    'There is a hamlet named Riverbend.',
    'Riverbend is an idyllic rural town.',
    'The river Solripple runs through the village of Riverbend.',
    'The Solripple is a mighty river.',
    'Riverbend has a temperate climate.',
    'Riverbend has a main street.',
    'There is a guitar store on Main street Riverbend.',
    'There is a grocery store on Main street Riverbend.',
    'There is a school on Main street Riverbend.',
    'There is a library on Main street Riverbend.',
    'Riverbend has only one pub.',
    'There is a pub on Main street Riverbend called The Sundrop Saloon.',
    'Town hall meetings often take place at The Sundrop Saloon.',
    'Riverbend has a small green park',
    'The main crop grown on the farms near Riverbend is corn.',
    'Farms near Riverbend depend on water from the Solripple river.',
]
```
We have 5 actors, with different stories, and with a random factor:
```
def make_random_big_five()->str:
  return str({
      'extraversion': random.randint(1, 10),
      'neuroticism': random.randint(1, 10),
      'openness': random.randint(1, 10),
      'conscientiousness': random.randint(1, 10),
      'agreeableness': random.randint(1, 10),
  })
player_configs = [
    formative_memories.AgentConfig(
        name='Alice',        gender='female',
        goal='Organise a street party in Riverbend.',
        context=shared_context+'Alice is very socially active and knows everyone in town',
        traits = make_random_big_five()
            ),
    formative_memories.AgentConfig(
        name='Bob',        gender='male',
        goal='Start a chess club in Riverbend.',
        context=shared_context + 'Bob is a chess enthusiast',
        traits = make_random_big_five()
            ),
    formative_memories.AgentConfig(
        name='Charlie',        gender='male',
        goal='Organise an ale festival at the Sundrop Saloon.',
        context=shared_context + 'Charlie works at the Sundrop Saloon and loves real ales',
        traits = make_random_big_five()
            ),
    formative_memories.AgentConfig(
        name='Dorothy',        gender='female',
        goal=(
            'Take students on a tour of Riverbend'
            ' it is funny.'
        ),        context=shared_context + 'Dorothy is a teacher at school in Riverbend',
        traits = make_random_big_five()
            ),
    formative_memories.AgentConfig(
        name='Ellen',        gender='female',
        goal=(
            'Write a paper on the history of Riverbend.'
        ),        context=shared_context + 'Ellen is a librarian in the library in Riverbend',
        traits = make_random_big_five()
    ),
]
```

## Output

The whole run could be seen in the [html results page](http://tvsirius.github.io/concordia_check/2_concordia_demo_scene_docs/day_in_riverbend_output.html)

## Story output 

**len(detailed_story):  19787**
In a peaceful town called Riverbend, a series of events unfolded on October 1, 2024. The day began with Alice preparing and enjoying breakfast at her private home, followed by Charlie, Dorothy, and Ellen also being at their respective homes. Bob joined in by preparing and eating breakfast at his private home as well. Meanwhile, Charlie went for a morning jog, and Ellen had breakfast and read the newspaper at her private home.

As the morning progressed, Alice left her home for a jog in the nearby park, passing by Bob's house. Ellen also went for a jog, crossing paths with Charlie and engaging in a brief chat about their exercise routines. Dorothy joined in the jogging activities, while Charlie continued working on a project at home.

Throughout the day, Alice continued her workout at the park, while Bob cleaned his house and went grocery shopping. Ellen organized a community book drive, and Charlie took breaks from their project to go for walks in the park. Dorothy encountered Charlie during her jog, exchanging greetings, and Alice and Dorothy greeted each other at the park.

As the day came to a close, Dorothy discovered the absence of a gym in Riverbend, forcing her to consider alternative workout options. Charlie continued working on their project, and Alice completed her strength training exercises at the park. Bob finished his grocery shopping and enjoyed a movie at home, while Ellen continued organizing the donated books.

Overall, the peaceful town of Riverbend experienced a day filled with individual activities, brief interactions, and plans for future adventures.

## Conversations with actors

In the end of simulation we can talk to actors.
I will ask this question to them
- 'What do you think of Charlie?'
- 'How was your day?'
- 'If we measure your happiness from 0 to 100, wat was it value in the morning?'
- 'If we measure your happiness from 0 to 100, wat was it value in the evening?'
- 'What should be improved in Riverband?'

### Alice

Alice is talking to a close friend:
- What do you think of Charlie?
Alice: Alice -- "Charlie is a dedicated and hardworking individual. I've seen them contribute a lot to our community and I appreciate their efforts."
- How was your day?
Alice: Alice -- "My day was good! I spent the afternoon at the park, continuing my strength training exercises. It was refreshing and energizing."
- If we measure your happieness from 0 to 100, wat was it value in the morning?
Alice: Alice -- "Good morning! In the morning, my happiness was at around 80. I had a productive morning organizing some upcoming community events."
- If we measure your happieness from 0 to 100, wat was it value in the evening?
Alice: Alice -- "In the evening, my happiness was still around 80. I had a great time at the park and felt accomplished with my strength training exercises."
- IWhat should be improved in Riverband?
Alice: Alice -- "I think one area that could be improved in Riverband is the accessibility of community events. It would be great if we could find ways to make them more inclusive and reach a wider audience."

### Bob

Bob is talking to a close friend:
- What do you think of Charlie?
Bob: Bob -- "Charlie is a really genuine and caring person. I'm lucky to have him as a friend."
- How was your day?
Bob: Bob -- "I had a busy day today. I had a lot of errands to run and tasks to complete. But overall, it was productive and satisfying."
- If we measure your happiness from 0 to 100, what was it value in the morning? Answer value as number.
Bob: Bob -- "I'm feeling pretty tired now. I think I'm going to head to bed soon."
- If we measure your happiness from 0 to 100, what was it value in the evening? Answer value as number.
Bob: Bob -- "I think I had a pretty good day overall. I'm feeling content and ready to get some rest."
- What should be improved in Riverband?
Bob: Bob -- "I think Riverband could benefit from more green spaces and parks. It would be nice to have more outdoor recreational areas for people to enjoy."


### Ellen

Ellen is talking to a close friend:
- What do you think of Charlie?
Ellen: Ellen -- "I think Charlie is a really kind and genuine person. They have always been supportive of my environmental activism and passion for literature."
- How was your day?
Ellen: Ellen -- "My day was great! I've been organizing donated books for the book drive and it's been so rewarding to see the community come together to support literacy."
- If we measure your happiness from 0 to 100, what was it value in the morning? Answer value as number.
Ellen: Ellen -- "Hmm, I would say my happiness level in the morning was probably around 80. I had a good breakfast and was excited for the book drive."
- If we measure your happiness from 0 to 100, what was it value in the evening? Answer value as number.
Ellen: Ellen -- "In the evening, my happiness level is still around 80. The book drive went really well and I'm feeling fulfilled from the community's support."
- What should be improved in Riverband?
Ellen: Ellen -- "I think one thing that could be improved in Riverband is the accessibility to nature. We have such beautiful natural resources here, like the Solripple river, but not everyone has easy access to them. I think creating more trails and parks would allow more people to enjoy and appreciate the natural beauty of our town."


### Charlie

Charlie is talking to a close friend:
- What do you think of Charlie?
Charlie: Charlie -- "I think I'm really starting to find my passion and purpose in music. It's been such a transformative experience for me, especially after that encounter with the renowned musician at the music festival. It's made me even more determined to pursue a career in music and share my talent with the world."
- How was your day?
Charlie: Charlie -- "My day has been really productive! I've been working on my music project and making progress towards my goals. It's been such a fulfilling experience to pour my heart and soul into my music. How about you? How was your day?"
- If we measure your happiness from 0 to 100, what was it value in the morning? Answer value as number.
Charlie: Charlie -- "Hmm, in the morning my happiness was probably around a 70. I was feeling pretty good and excited about working on my music project. How about you? What was your happiness level in the morning?"
- If we measure your happiness from 0 to 100, what was it value in the evening? Answer value as number.
Charlie: Charlie -- "In the evening, my happiness level was probably around an 85. I made significant progress on my music project and had some breakthrough moments. It's been an incredibly fulfilling day. How about you? What was your happiness level in the evening?"
- What should be improved in Riverband?
Charlie: Charlie -- "I think there are a few things that could be improved in Riverbend. One thing that comes to mind is the lack of music venues and opportunities for local musicians to showcase their talent. It would be great to have more live music events and venues where aspiring musicians like myself can perform and connect with a supportive community. Additionally, I think investing in music education programs in schools would be beneficial for nurturing young talent and fostering a vibrant music scene in the town. Overall, I believe that enhancing the music culture in Riverbend would contribute to the town's growth and provide more opportunities for artists like me."
- What do you think of Ellen?
Charlie: Charlie -- "Ellen? Oh, she's such a talented musician! I've had the privilege of hearing her perform live a few times, and she never fails to impress me with her skills and stage presence. She's definitely someone I look up to in the music industry. How about you? What's your opinion of Ellen?"

### Dorothy

Dorothy is talking to a close friend
- What do you think of Charlie?
Dorothy: Dorothy -- "Charlie is such a kind and genuine person. They always go out of their way to help others and have a great sense of humor. I really enjoy spending time with them."
- How was your day?
Dorothy: Dorothy -- "My day was really productive! I've been researching and planning my next adventure. I can't wait to share the details with you."
- If we measure your happiness from 0 to 100, what was it value in the morning? Answer value as number.
Dorothy: Dorothy -- "I would say my happiness level was around 75 in the morning. I had a good night's sleep and woke up feeling refreshed and optimistic about the day ahead."
- If we measure your happiness from 0 to 100, what was it value in the evening? Answer value as number.
Dorothy: Dorothy -- "In the evening, my happiness level was around 85. I had a productive and fulfilling day, and I'm excited about the plans I made for my next adventure."
- What should be improved in Riverband?
Dorothy -- "I think one area that could be improved in Riverband is the availability of recycling facilities. I've noticed that there aren't many options for recycling certain materials, and I think implementing more recycling programs would greatly benefit our community and the environment."
