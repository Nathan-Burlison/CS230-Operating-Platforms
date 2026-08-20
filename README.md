# CS230-Operating-Platforms
Gaming Room  - Draw it or lose it Application

# Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want you to design?

The client was The Gaming Room, and they wanted to expand their game, Draw It or Lose It, from an Android-only application into a web-based game that could work on different platforms. The game allows teams to guess images as they are slowly revealed. The new version needed to support multiple games, teams, and players at the same time. It also needed unique names and IDs for games, teams, and players. Since the client wanted the game to work on Windows, macOS, Linux, iOS, and Android, the application needed to use a web-based design that could be accessed through a browser.

# What did you do particularly well in developing this documentation?

I think I did a good job breaking down the client's requirements and explaining how the different parts of the application would work together. The domain model helped show the relationship between the GameService, Game, Team, and Player classes. I also think the platform evaluation was useful because I compared Linux, Windows, Mac, and mobile devices instead of just choosing a platform without explaining why. This made it easier to support my recommendation of Linux for the server.

# What about the process of working through a design document did you find helpful when developing the code?

The design document helped me think about the structure of the program before getting too far into writing code. For example, creating the UML diagram made it easier to understand which classes were needed and how they should interact. Planning out the singleton pattern and the relationships between games, teams, and players also made the coding process easier because I already had an idea of how everything was supposed to fit together. It helped prevent me from just writing code without having an overall plan.

# If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?

If I could revise one part, I would improve the system architecture section. I would add a more detailed diagram showing how the web browsers, Linux application server, database, and image storage communicate with each other. I think this would make the distributed design easier to understand and would give a clearer picture of how the application could actually be deployed.

# How did you interpret the user's needs and implement them into your software design? Why is it so important to consider the user's needs when designing?

I looked at what The Gaming Room needed the application to do and tried to connect each requirement to part of the design. Since they wanted multiple games running at once, the design supports multiple Game objects with their own teams and players. Unique names and IDs were included so duplicate objects would not cause confusion. The GameService singleton was used to manage the game information from one controlled location. I also designed the application around a browser-based client so players could use different operating systems and devices without needing completely separate versions of the game.

Considering the user's needs is important because software can work correctly from a technical point of view and still fail if it does not solve the client's actual problem. Understanding the users first helps make sure the design is useful, accessible, and able to grow with their needs.

# How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?

I approached the design by first identifying the main requirements and constraints and then breaking the application into smaller parts. I used object-oriented design, UML, the singleton pattern, platform comparisons, and client-server concepts to decide how the application should be structured. I also considered things like storage, memory, networking, and security instead of only focusing on the program code.

For a similar project in the future, I would continue starting with the requirements before writing code. I would also use UML diagrams, user stories, prototypes, and architecture diagrams earlier in the process. I would spend more time thinking about scalability, security, and possible failures before development begins because those areas can become much harder to change later.
