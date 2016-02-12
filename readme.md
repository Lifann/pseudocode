# Pseudocode

## Learning Objectives
- Describe the role of pseudocode in development
- List the steps for problem solving
- Create pseudocode to describe a basic problem


## What is pseudocode? (10 min)

According to wikipedia, [pseudocode is](https://en.wikipedia.org/wiki/Pseudocode):
> Pseudocode is an informal high-level description of the operating principle of a computer program or other algorithm.

> It uses the structural conventions of a programming language, but is intended for human reading rather than machine reading.

This is a great opportunity to turn tech speak in, well, human speak.

Let's break that down and translate it.

Q. What does that mean?
---

> A. Pseudocode attempts to be a way to describe a the solution to a problem, that is easier and more concise than code.  It a stepping stone toward writing the code.

I've heard Washington, DC described as where Northern hospitality meets Southern efficiency.

Pseudocode lives in that "in between" place too.  It has more logic than English, without all the structure of code.


### We Do: What does that look like? (15 min)

Pseudocode should describe the entire logic of the algorithm so that programming becomes a task of translating line by line of pseudo code into real code.

For each of following, let's discuss why each one could be considered "Good" or "Poor" examples of pseudocode:

**1. Problem - Determining If a Number is Even or Odd**

***Example 1:***
```
PROGRAM IsEvenOrOdd:
  var num = number;
  IF (num / 2 === 0)
    THEN Print "even";
    ELSE Print "odd";
  ENDIF;
END.
```
>This is not a great example. Here we are using "var" in our pseudocode when it should read plain english! Also, we should not be using the javascript syntax "===" in our conditional.

***Example 2:***
```
PROGRAM IsEvenOrOdd:
  Read number;
  IF (number divided by two has no remainder)
      THEN Print the number is even;
      ELSE Print the number is odd;
  ENDIF;
END.
```

**2. Problem - How to Make a PB&J Sandwich**

***From [Get Creative Today](http://getcreativetoday.com/lessons/pseudo-code-flowcharts/)***

***Example 1:***
```
Make PB&J Sandwich:
  Gather bread, peanut butter and jelly.
  Apply peanut butter to slice of bread.
  Apply jelly to another slice of bread.
  Bring to two slices of bread together.
  Eat and enjoy.

```
>Although this might appear to be a good set of instructions and intuitive for us to follow, we need to break these down into smaller steps for the computer to understand.

***Example 2:***
```
PROGRAM MakePB&JSandwich:
  Grab a paper plate;
  Open bread container;
  Grab bread package;
  Untwist bread package;
  Open bread bag and remove two slices;
  Place slices on paper plate;
  Grab a plastic knife;
  Open peanut butter jar;
  Use knife to scoop out peanut butter;
  Apply peanut butter to one slice of bread;
  Spread peanut butter on slice;
  Place knife on plate;
  Close peanut butter jar;
  Open jelly bottle;
  Squeeze jelly onto second bread slice;
  Close jelly bottle;
  Place down jelly;
  Pick up knife;
  Spread jelly on slice;
  Bring two slices of bread together;
  Cut slices in half down the middle;
  Throw knife in the trash;
  Pick up one half of sandwich;
  Enjoy;
END.  
```
>This example's sequence is very thorough! However, we are still assuming certain conditions that our utensils or ingredients already exist. What if we are out of plates? Will we grab a napkin instead to place our sandwich on? What if we are out of jelly? Will you throw the sandwich away or eat it with just peanut butter?

Computers are not smart. We need to give them step by step instructions to account for conditions. They can not adapt to make changes without being explicitly told. Programing is a series of tasks, which can be completed only if a certain number of conditions are met.


## Exercise: Draw Toast (30 min)

Got a wicked problem? First, tell me how you make toast.

https://github.com/ga-wdi-exercises/draw_toast

## Break (10 min)

## Exercise: Solve the Waiter Problem (5 min)

Using your new found skills, solve this:

- A waiter has N tables, each with 2-4 guests.
- The waiter makes rounds between each of their tables, the bar, and the kitchen.
- The waiter takes drink orders for a new table, then submits them to the bar.
- Drinks are delivered when all table orders are ready.
- The waiter takes food orders for a new table, then submits them to the kitchen.
- Food is delivered when all table orders are ready.
- The waiter checks idle tables for additional requests, then submits them appropriately.
- Additional requested items are delivered when all table orders are ready.


Q. In one sentence, what problem were you solving?
---

> A. Discuss the answers and the importance of identifying the problem.

We realize you didn't have enough time to solve it.  We hope that, through this exercise, you learned the importance of clearly identifying the problem.

## Approaching a coding problem (15 min)

Before we can write pseudocode to solve the problem, we need to know the problem.  

Here are some steps that can help:

- Identify the Problem
- Conceptualize
  - Big picture, big strokes
- Break it down
- Start small

### Identify the Problem

- What exactly are we trying to solve?  - From who's viewpoint?  
- Who will benefit?  
- What are we delivering?

### Review: the Steps

- Identify the Problem
- Conceptualize
  - Big picture, big strokes
- Break it down
- Start small

Q. Where does pseudocode fit?
---

> A. Break it down OR Start small

This process is iterative.  We keep circling around and repeating the earlier steps, just at a different level.

When we first approach a problem, we see the big picture.  "Break it down" gives us big steps.  Then, we take one of those steps and "Break it down".  Now, starting small, we write pseudocode to help illustrate the problem.  

Pseudocoding proves that we have *identified* the problem, understand it *conceptually*, and have *broken it down* into *small steps* that we can follow.


## Syntax for Pseudocode:

There is no one, fixed syntax for pseudocode.  It just needs to be clear, simple, and concise.  

If you feel stuck, feel free to use this syntax:

***Referencing: [Introduction to Pseudocode](http://www.slideshare.net/DamianGordon1/pseudocode-10373156)***

* General Structure of Pseudocode
  ```text
  PROGRAM <ProgramName>:

  <Do Stuff>

  END.
  ```

* Selection: IF/ELSE Statements
  ```
  IF (<Condition>)
    THEN <Statements>;
    ELSE <Statements>;
  ENDIF;

  ```
* Iteration: LOOP
  ```
  WHILE (<Condition>)

  ENDWHILE;
  ```

## Exercise: If there are eggs

A programmer is going to the grocery store and his wife tells him, "Buy a gallon of milk, and if there are eggs, buy a dozen."

So the programmer goes, buys everything, and drives back to his house.

Upon arrival, his wife angrily asks him, "Why did you get 13 gallons of milk?"

The programmer says, "There were eggs!"

### We Do: Only milk (10 min)

1. Write the pseudocode that shows why he only bought milk.

### You Do: Milk and eggs (15 min)

1. Write pseudocode that gets me (errr...  um...  THAT programmer) to buy milk and eggs.

## Break (10 min)

## Exercise: Pseudocode FizzBuzz (30 min)

Break into small groups and solve this puzzle:

You're given a robot. The robot has no imagination or creativity whatsoever, but it's good at following rules.

The robot can only obey 9 commands:

- Add two numbers together
- Subtract two numbers
- Multiply two numbers
- Divide two numbers
- Find the remainder of one number divided by another
- Remember a number
  - For example, "Number A is 42"
- Say something
- Go back to an earlier step in the instructions
- Tell if two numbers are equal, and if they are do one thing, and otherwise do another thing
  - For example, "If Number A equals 42, say 'Hello'. Otherwise, go back to step 3."

You need to write a list of instructions for the robot so that when it's given a number &mdash; say, 73 &mdash; for each number between 1 and 73:

- If the number is divisible by 3 it says "Fizz"
- If the number is divisible by 5 it says "Buzz"
- If the number is divisible by 3 and 5 it says "FizzBuzz"
- If the number isn't divisible by 3 or 5 is says the number

So if the number was 9, the robot would say:

```
"One"
"Two"
"Fizz"
"Four"
"Buzz"
"Six"
"Seven"
"Eight"
"Nine"
```

To start, consider:

- How would you get the robot to count to 73? You can't just say, "Count to 73." That's not one of the commands the robot knows. Of the 9 commands you've been given, which might be helpful?

- How can you tell if one number is divisible by another? (For example, 8 is divisible by 2, but not by 3.)
