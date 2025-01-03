# Unexpected Immutability of Instance Variables in Ruby

This repository demonstrates a common pitfall in Ruby where instance variables appear immutable if a setter method is not explicitly defined.

The `bug.rb` file showcases the issue, while `bugSolution.rb` provides a solution demonstrating how to correctly define a setter method.

## Bug Description

When you create instance variables in Ruby and do not provide explicit setter methods, attempts to modify their values from outside the class will fail silently. The variable will retain its initial value.

## Solution

To resolve this, create a `value=` method (or a similarly named method based on your instance variable). This will enable modification of the instance variable from outside the class.
