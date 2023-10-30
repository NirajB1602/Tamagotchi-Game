# Tamagotchi Game Project

## Project Overview
Do you remember those cute little electronic pets, Tamagotchis? They were these adorable creatures that needed your care. Over time, they would get hungry or bored, and if you didn't tend to them, they'd get sick. All of this was managed with just a few buttons on the device.

Now, we're going to create a simplified, text-based version of that experience. In our problem set and during our exploration of Inheritance, we'll take this further.

Let's start with a class called Pet. Each instance of this class will represent one electronic pet for you to take care of. These digital companions will have a current state, which includes three things:

- Hunger (an integer)
- Boredom (an integer)
- Sounds (a list of strings, like words the pet has learned to say)

In the __init__ method, we'll set hunger and boredom to random values between 0 and the point where they'll start feeling hungry or bored. The sounds instance variable will be initialized with a copy of the class variable with the same name. We're making a copy because we'll be making changes to this list, and we don't want those changes to affect the list pointed to by the class variable.

We've also got a clock_tick method. It'll increment the boredom and hunger instance variables, simulating the idea that as time passes, the pet gets hungrier and more bored.

The __str__ method will produce a string that tells us the pet's current state. It'll let us know whether it's bored, hungry, or happy. Boredom is considered if the boredom instance variable exceeds a certain threshold, which is set as a class variable.

To help relieve boredom, the pet owner can teach the pet new words using the teach() method or interact with the pet using the hi() method. When the pet learns a new word, it adds it to its list of known words. When you say "hi" to the pet, it will respond with one of the words it knows, randomly picking one from its list. Both hi() and teach() will decrease the boredom state by an amount defined in the class variable boredom_decrement. The boredom state can't go below 0.

To address hunger, we have the feed() method.

Now, that's all excellent if you want to interact with the pet by writing Python code. But let's take it up a notch and create a game that anyone, even non-programmers, can enjoy.

We'll use the Listener Loop pattern. In this game, at each step, we'll display a text prompt to remind the player of what commands they can use.

The player will have a list of pets, each with a unique name. They can issue commands to adopt new pets, creating new instances of the Pet class. Or they can interact with their existing pets using Greet, Teach, or Feed commands.

No matter what the player does, with each command entered, time will pass for all their pets. Be careful, though; if you have too many pets, you might find it challenging to keep them all happy and satisfied!

## Project Description

The project encompasses the following key components:

1. **Virtual Pet Creation**: Players can create their virtual pets by selecting different types, colors, and names for their digital companions. Each pet has its unique characteristics and needs.

2. **Pet Care Activities**: Players are responsible for taking care of their virtual pets. They can feed them, play with them, and ensure their health and happiness.

3. **Life Stages**: Virtual pets go through different life stages, from birth to aging. Players need to adapt their care routines based on the pet's life stage.

4. **Pet Interaction**: Players can interact with their virtual pets, creating a bond and improving their pet's mood. Neglecting their pets can lead to unhappiness and even loss.

5. **Score and Achievements**: The game may include scoring and achievements based on how well players take care of their virtual pets. Achieving high scores can unlock new features or pet types.

6. **Game Over Conditions**: The game should have conditions that lead to a "Game Over" state, such as the pet getting sick or unhappy due to neglect. When this happens, players have the option to start a new game.

7. **User Interface**: The project includes a user-friendly interface for players to interact with their virtual pets. This can be a mobile app, a web application, or a desktop game, depending on the implementation.

8. **Documentation**: A comprehensive project documentation, including the README.md file, describes the project, its components, and how to play the game.

## Contributors

- [Niraj Bansal](https://github.com/NirajB1602)

Feel free to fork, contribute, and share this project with others who share an interest in virtual pet simulation games and game development.
