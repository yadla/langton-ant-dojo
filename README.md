# Dojo : TDD Against the Time with React and Redux

## What is the Langton's Ant ?
__Langton's ant__ is a two-dimensional universal Turing machine with a very simple set of rules but complex emergent behavior. It was invented by Chris Langton in 1986 and runs on a square lattice of black and white cells. The universality of Langton's ant was proven in 2000. The idea has been generalized in several different ways, such as turmites which add more colors and more states.

### How it works ?
Squares on a plane are colored variously either black or white. We arbitrarily identify one square as the "ant". The ant can travel in any of the four cardinal directions at each step it takes. The "ant" moves according to the rules below:
* At a white square, turn 90° right, flip the color of the square, move forward one unit
* At a black square, turn 90° left, flip the color of the square, move forward one unit

Langton's ant can also be described as a cellular automaton, where the grid is colored black or white and the “ant” square has one of eight different colors assigned to encode the combination of black/white state and the current direction of motion of the ant.

## Dojo's rules
### TDD
Test-driven development (TDD) is a software development process that relies on the repetition of a very short development cycle: Requirements are turned into very specific test cases, then the software is improved to pass the new tests, only. This is opposed to software development that allows software to be added that is not proven to meet requirements.
![TDD Cycles](https://upload.wikimedia.org/wikipedia/commons/0/0b/TDD_Global_Lifecycle.png)
5 Steps to reproduce every cycle:
1. Add a new test
1. Run all tests and verify if the new test fails
1. Write code to pass the new test to green
1. Run all tests and verify all are green
1. Refactor

For more informations, see [Wikipedia](https://en.wikipedia.org/wiki/Test-driven_development)

### TDD Against the Time
In this type of sessions, we add one key constraint on the TDD cycle : Before each test, we launch a five minutes timer.
* If the code compiles and the tests are green, commit!
* Otherwise, revert!

The five minute time constraint sounds fiendish doesn’t it? How can you possibly get anything done in five minutes? Well, you can, if you tackle something small enough. This exercise is designed to force you to think in small increments of functionality.


### BDD
Behaviour-Driven Development (BDD) is a set of practices that aim to reduce some common wasteful activities in software development:
* Rework caused by misunderstood or vague requirements
* Technical debt caused by reluctance to refactor code
* Slow feedback cycles caused by silos and hand-overs

BDD aims to narrow the communication gaps between team members, foster better understanding of the customer and promote continuous communication with real world examples.

![BDD](./images/bdd.png)

### Example mapping
Example Mapping is a simple method to make this conversation short and very productive.

Concrete examples are a great way to help us explore and understand the problem domain. They are a great basis for our acceptance tests.

When discussing examples, other things might come up in the conversation that deserve to be captured too:
* rules that summarise a set of examples, or express other constraints.
* questions that cannot be answered during the conversation, or assumptions that are made.
* new user stories discovered or sliced and deferred out of scope.

We can capture these different types of information on index cards, and arrange them in a map:
* We write the story on a yellow card and place it on top.
* Each of the acceptance criteria, or rules, is written on a blue card and placed beneath the yellow story card.
* Examples to illustrate these rules are written on a green card and placed under the relevant rule.
* Questions that cannot be answered during the session are captured on a red card so we can move on with the conversation.

We keep going until the group is satisfied that the scope of the story is clear, or we run out of time.



### Code coverage
All __your__ code must be covered by unit tests. Our technology permit this : React, TypeScript, Jest and Enzyme.

### Types
In this case, we'll use Typescript to verify coherence between objects. We'll avoid maximum `any` (implicit or not).

## Steps
It is a six parts dojo, each part need previous (or previous solution) to be played :
1. [Create React Project](./STEP_1.md)
1. [A Grid and An Ant](./STEP_2.md)
1. [First rules and Component State](./STEP_3.md)
1. [From Component State to Redux](./STEP_4.md)
1. [Asynchronous logic with Redux](./STEP_5.md)
1. [Advanced Typescript and React Forms](./STEP_6.md)

> Now we can begin the dojo with the [first step : Create React App](./STEP_1.md)
