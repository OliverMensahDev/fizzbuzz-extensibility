## Problem

Mostly coding up fizzbuzz solution is easier by just returning some value when requirements are met. Then a new requirement comes that says replace all numbers divisible by 7 with `Whizz`. All we mostly do is just adding one more check then return what is needed to. It is good that way but it does not improve the design of our code and also violates software design principles like Open/Closed Principle(OCP) of the SOLID principle.

## Solution

You can adhere to the OCP principle by removing specifics from the FizzBuzz class using interface. The specifics here are matching condition and replacement of value. Then let each specific implement the interface and then inject all the specifics to the fizzbuzz class

## Benefits

1. Less code modification in the main class(FizzBuzz)
2. Easier to add more specifics
