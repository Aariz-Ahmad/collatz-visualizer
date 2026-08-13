# Collatz Visualizer

A visual experiment with the Collatz sequence.

This project isn't a mathematical testing tool, and it isn't intended to contribute to research on the Collatz conjecture. I made it because I find something about these sequences genuinely beautiful: an extremely simple set of rules can produce behavior that looks incredibly complicated.

The visualizer takes a starting number, generates its Collatz sequence, and turns that sequence into a path. Each number becomes a node, and the resulting path is arranged into a growing spiral.

The point isn't to prove anything. It's to see the patterns.

## The idea

The Collatz sequence is generated using a very simple rule. If a number is even, divide it by two. If it is odd, multiply it by three and add one.

Despite how simple that is, the sequences can behave in surprisingly complicated ways.

I wanted to represent that visually rather than just looking at a list of numbers. Every value in the sequence becomes a node, with consecutive values connected by line segments. The result is a geometric representation of the sequence itself.

The current version uses a turtle-style system to arrange the nodes into a growing spiral. The turtle has a position, heading, and step length, with those values changing as the sequence progresses.

## Why I made it

I'm fascinated by the way patterns can emerge from very simple systems.

Math has a lot of examples of this, but the Collatz sequence is one of the ones that really captures it for me. There isn't a complicated rule telling the sequence to form interesting structures. The rules are almost absurdly simple, yet when you follow them, patterns emerge.

That's what I wanted to capture with this project.

## The visualization

The spiral isn't meant to represent some hidden mathematical property of the Collatz conjecture. It is simply a visual language for displaying the sequence.

The spacing between nodes, rotation of the spiral, animation, and camera behavior are all designed around making the structure easier and more interesting to look at.

One of the problems I ran into was preventing the main path from crossing itself. The current approach uses straight segments and adjusts the growth of the turtle's step as the spiral expands.

The final `4 → 2 → 1` cycle is also represented explicitly.

## Current state

Still in development.

I'm continuing to experiment with the geometry, spacing, animation, and different ways of representing the sequences.

## Built with

HTML, CSS, and JavaScript.

The sequence calculations use JavaScript `BigInt` so the visualizer isn't limited by normal JavaScript integer precision.

## AI use

AI was used in a small part of this project for debugging and working through a few implementation problems.

The visualization, design, and underlying approach are my own.
