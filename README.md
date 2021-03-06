# Refactoring-CodingChallenge

This is refactoring coding challenge that I developed to show you my coding and design skills:

1. [Guice](https://github.com/Vedenin/RockPaperScissorsCodingChallenge/blob/master/src/main/java/com/github/vedenin/testtask/ApplicationModule.java),
2. [Dependency injection](https://github.com/Vedenin/RockPaperScissorsCodingChallenge/blob/master/src/main/java/com/github/vedenin/testtask/ApplicationModule.java),
3. [Pattern Strategy](https://github.com/Vedenin/RockPaperScissorsCodingChallenge/tree/master/src/main/java/com/github/vedenin/testtask/strategies)
4. [SOLID principle](https://github.com/Vedenin/RockPaperScissorsCodingChallenge/tree/master/src/main/java/com/github/vedenin/testtask)
5. [TestNG](https://github.com/Vedenin/RockPaperScissorsCodingChallenge/tree/master/src/test/java/com/github/vedenin/testtask)
6. [TDD principle](https://github.com/Vedenin/RockPaperScissorsCodingChallenge/tree/master/src/test/java/com/github/vedenin/testtask)

## Coding Challenge Requirements

Coding Example
- The programming language is Java.
- The code is to be tested.
- Please submit code as well tests.
- Please describe shortly the advantages and disadvantages of your design.
- The IDE is free to choose
- The build tool should be Maven or Gradle, but can be different.
- Please solve this task according to the standards like you would in your normal work.

Task: Rock-Paper-Scissors

Build a game in which two players compete in a game of Rock-Paper-Scissors with different strategies. Who will win more rounds? The rules:

- Scissors beats Paper

- Rock beat Scissors

- Paper beats Rock

- If both players choose the same, the round is counted as a tie.

Implement two players:

- Player A always chooses Paper

- Player B chooses randomly

The game consists of 100 rounds of above two players competing. The output of the program

should be like the following:

"Player A wins 31 of 100 games"

"Player B wins 37 of 100 games"

"Tie: 32 of 100 games"

## About Systems

Coding Example
Task: Rock-Paper-Scissors

Build system: maven
Test system: TestNG

Pattern: Strategy, Dependency injection

Run:
1. Build project using maven
2. Run main method of Application.class (package com.github.vedenin.testtask)

Testing:
1. StrategiesTest - test all Strategies
2. RulesTest - test rule of Rock-Paper-Scissors
3. GamesTest - integration test of all project

Advantages of my design:
1. Using single responsibility principle (every class have only one task)
2. Using open/closed principle (easy for extension, almost all class has interface)
3. Dependency inversion principle (using Dependency injection framework - Guice)
4. Possible to extensions for any Two-player games (chess, checkers, go and so on)
5. Only some class has specific Rock-Paper-Scissors details (in package rockpaperscissors),
other classes can be using in any Two-player games

Disadvantages of my design:
1. Many class/interface for extensions for any Two-player games
