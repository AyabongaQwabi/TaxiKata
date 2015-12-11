# Taxi Kata

## Instructions

Solve the Kata below using TDD. Complete it in Javascript, Python, or Ruby. Once done in one Language in the alotted time try it out in another. Use flowcharts and diagrams to think through the required logic.

## Part 1

A taxi boss wants to gather statistics on their rank: they want to see how quickly taxis move through the rank, and how long people usually wait.

* Create a `Rank` class. The constructor should specify the **number of taxis** at the rank and the **number of people** waiting.
* Create a `Taxi` class. The constructor should specify the **number of passengers** allowed on the taxi.

People board the `Taxi` using the `load` method. Multiple people can board at the same time.

The `Rank` keeps track of how many people are there using the `people` property, and of how many taxis are there using the `taxis` property.

When a taxi is full, it leaves the `Rank` using the `leave` method.

## Part 2

## Destination

* Extend your `Taxi` class by adding a `destination` property.
* Create a `Group` class. The constructor should have the **number of people** in the group, and their **destination**.
* Update your `Taxi` class to only let on people going to the same destination as the taxi.

## Code Coverage

Code coverage tells you how much of your code is covered by your tests. Higher code coverage can mean your code has a good chance of being well-tested and contain few bugs.

Let's use a tool called [Instanbul](https://gotwarlost.github.io/istanbul/) to check our code coverage.

### Istanbul

Install Istanbul globally like this:

```
$ npm install -g istanbul
```

To run Istanbul's coverage calculation with your mocha tests, run:

```
istanbul cover _mocha
```

Instanbul generates a web page of the detailed results of its calculations to `coverage/lcov-report/index.html`. Look at this page to see which particular bits of your code aren't being covered by your tests.
