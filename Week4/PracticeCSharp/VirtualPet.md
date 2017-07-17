# Virtual Pet

## Overview
Create a console application for an interactive game-like virtual pet program. The user must be able to select different tasks or activities from a menu.

## Skills Required
-  Methods
-  Intro to OOP


## Tasks
- [ ] VirtualPet class
  - [ ] Find all comments with TODO and follow the instructions listed
  - [ ] Fields (at least three)
  - [ ] Methods (at least three)
  - [ ] Constructors (at least one)
- [ ] Program class
  - [ ] `Main` method
    - [ ] Find all comments with TODO and follow the instructions listed
    - [ ] Interactive user interface (see example at bottom of page)
      - [ ] Continue building a menu for user interaction
      - [ ] Display current status of pet
      - [ ] Display options for interacting with pet
      - [ ] Ask user what action to take
        - [ ] User's selection should trigger an action

## To Start the Project
In order to do this project, you need to download the [Template for VirtualPet](https://github.com/WeCanCodeIT/VirtualPet_Template). To download this project, click on the green button that says *Clone or download*. In the future, we will learn how to clone projects, but for now, choose the *Download ZIP* option. Once you have downloaded the Template, right click on the zip file and choose "Extract All". If your computer prompts you to choose a location for the folder, please choose your *Projects* folder inside your *Visual Studio 2015* folder. Reach out to an Ed Team member if you need help with this process. You should then be able to open the template and begin working.

## Details

Make a virtual pet program. This is your version of a Tamagotchi or DigiPet!

This might seem like a daunting task, but we can break it down.

To find the tasks on the project that need to be completed, search the document (`Ctrl + f`) for any comments that start with *"TODO"*

First, decide what "features" you want to incorporate. You might be tempted to make this a long list - start small! Think MVP!

Next we'll be following a template of a class for the pet. Think of what fields/methods you will need to have for your MVP. Methods might involve things that happen when a person interacts with the pet.


Some ideas for things that a virtual pet should have (along with some ideas for activities that might address them):

- Hunger (Feed it)
- Thirst (Water it)
- Waste (Let it out to the bathroom)
- Boredom (Play with it)
- Sickness (Take it to the doctor)

*Note*: You do not have to include all of the above fields and methods, you can narrow it down to three.

Your methods should cause the appropriate fields to update - for instance, if you have a `Feed()` method, it might make `Hunger` go down, but make `Thirst` go up.

Other fields that might update:
  - boredom increasing
  - hunger increasing
  - sleepiness increasing

If you play with the pet, perhaps that makes it more tired but boredom goes down. Have fun with this part!

Also, remember that more features `!=` better. Pick a focus for your pet. Maybe go with a theme.

Once you've designed the class, it's time to think about the user interface. We're using a Console interface for now, so it will likely involve some sort of loop and a menu showing possible actions, as well as indicating the state of the pet. 

Your user interface should live in the `Main` method of the `Program` class. You should also have a `VirtualPet` class in a separate file.

An example user interface is below (you do not have to make yours match this!):

```
Horace the Hippo
Hunger: 27
Thirst: 5
Boredom: 5
Tiredness: 50

What do you want to do?
1. Feed Horace
2. Water Horace
3. Play with Horace
4. Put Horace to sleep
5. Do nothing

> 1

You feed Horace.
```

## Stretch Tasks
- [ ] Give the pet the ability to take care of some of its own needs
- [ ] A visual representation of the pet
- [ ] Alternative interfaces
- [ ] You can try to include a method called `Tick()` that will update any properties or call time-based methods. The idea behind this method is that every time the menu is shown or some user interaction occurs, you could call the `Tick()` method to cause properties to update. You may want to have some of the properties update randomly to make the virtual pet less predictable.
- [ ] Calling `Tick` in a separate thread

Pets are not robots - they usually have some sort of self-determination! When `Tick` is called, you might want to have your pet take a look at its needs and possibly address one. You could use a random number generator to have it do things randomly, or prioritize things based upon what need is highest. You could also make your pet uncooperative - when the user tries to feed the pet, for example, you might make the pet refuse to eat.

Rather than using numbers to convey your pet's status, you could have some sort of visual representation of the pet. I.e., instead of printing `hunger: 50`, you could use smileys or [ASCII art](https://en.wikipedia.org/wiki/ASCII_art) to show hunger when `hunger >= 50`.
```
     >=<        
,.--'  ''-.
(  )  ',_.'
Xx'xX      

Horace looks like this: :0

1. Feed Horace
2. Water Horace
3. Play with Horace
4. Put Horace to sleep
5. Do nothing
```

Consider exploring threads and how you could have `Tick` occur every second, rather than waiting for user input.


## Hints
Don't try to tackle everything at once! Break this project up into smaller chunks, and you will find that they are all manageable.
