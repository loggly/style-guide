---
title: loggly engineering style guide
layout: default
---

# General Style Guide

Overal goals:

* Consistency is important.
* Code should be readable and maintainable.
* Documentation should be readable and maintainable.

Code reviews should serve as a point of learning and enforcement of consistent style.

## Language specifics

Don't write Python like Java. Don't write Java like JavaScript. Each has
different styles already in our code, follow them where sensible and update
this document accordingly.

In Python, follow PEP8 when possible.

## Variable names

Be verbose. Make them meaningful and readable.

Short iterator variables (in loops) are acceptable if the loop body is small

For nested loops/iterations, you must name all variables as you would any other (not short single-letters).

### Example of what not to do

This is hard to read:

    for i in foo:
        for i1 in bar:
            for i2 in baz:
                if i1 == i:
                  print i2

Above: Surely these 3 'i' values have meaning. Give them names.
