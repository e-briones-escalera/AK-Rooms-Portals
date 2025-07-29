## Dev Diary: Behind the Build
First I would like to thank you for reading this diary, I wanted to structure it like a blog, so it is easier to understand all of my notes and thoughts about this game. 

>  Note: The videos are at the bottom of [this webpage](https://www.9csound.com/game-audio)

### Context & Challenges  

When we received this project, we knew it was going to be a real challenge. Not every team had the same game, and ours was considered one of the hardest projects because it was extremely buggy, which affected everything,
including the audio integration. Besides implementing the audio in Wwise, we also had to debug multiple issues in Unity that weren’t even related to our work. The game would crash or freeze more often as we added extra features, 
which made the process of connecting events and validating our work much harder.  

### Why AK Rooms & Portals?  

Since the game takes place in a sort of spaceship/advanced control center, with rooms of very different sizes —some huge and others very small—, it was important that players could *feel* the difference in scale as they moved 
through the environment.  

That’s why I decided to learn Wwise AK Rooms & Portals from scratch. I even went through the full tutorial to fully understand how it worked. My main goal was clear:  
- Make the audio reflect the size and connectivity of each space.
- Small rooms should feel tight and closed.  
- Large rooms should feel expansive and open.  

### Implementation  

- Created Rooms for each major area in Unity and connected them with Portals for accurate sound propagation.  
- Carefully linked portal states with doors and level geometry, so audio would dynamically adapt when doors opened or closed.  
- Designed custom reverb zone for each room to match its size and materials, giving each space its own acoustic identity.  
- Debugged complex overlapping areas and manually adjusted portal positions to avoid audio leaks or unnatural transitions.  

### Debugging & Problem Solving  

Implementing Rooms & Portals in a bug-heavy project wasn’t easy:  
- Some Unity collisions and triggers were broken, so we had to manually create additional debug tools to visualize which room/portal the player was in.  
- We logged room transitions and active portals in real-time to quickly detect inconsistencies.  
- Adjusted audio priorities and occlusion values to maintain consistent performance despite the high number of audio sources.  

These debugging steps were crucial to making the system stable and functional in a very unstable game build.  

### Results  

Even though the process was challenging, implementing AK Rooms & Portals completely changed the perception of space in the game:  
- Each room now feels unique, and players can sense when they enter a large, open hall versus a small, enclosed chamber.  
- Sounds naturally propagate from one area to another, making the world feel more connected and alive.  
- The audio system now adds a layer of immersion that complements the gameplay instead of being just a background element.  

This was my first time using Wwise AK Rooms & Portals, and the learning experience was absolutely worth it.  


