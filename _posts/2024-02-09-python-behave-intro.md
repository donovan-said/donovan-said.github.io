---
title: Python behave, Dipping Our Toes In
tags: [Testing, Python behave, Gherkin]
style: fill
color: success
description: An introduction to Python Behave.
---

## What is Python behave?

Python behave is a Behaviour driven development (BDD)

[behave - Read The Docs](https://behave.readthedocs.io/en/latest/)

## Scenario

To keep thins simple, I've used a very basic scenario, which hopefully, shows you how simple this can be to set up, but
also how this can be expanded to perform more complex testing.

* Scenario: Check to see if a given endpoint returns an HTTP response code of 200.
* [Source Code](https://github.com/donovan-said/python-behave-examples/tree/main/behave/intro-blog-post/features)

## Setup

You first need to install [behave](https://pypi.org/project/behave/). I suggest that this forms part of your Pipfile;
here's an [example](https://github.com/donovan-said/python-behave-examples/blob/main/Pipfile) of this.

## Basic Structure

The basic structure for a behave directory comprises the root behave path, the features path, which contains your
environment.py and your feature files, and finally a steps path, which contains the steps python scripts actually
performing the defined tests. These will all be discussed in more detail in the following sections.

Below is an example of this:

```shell
└── behave
    └── features
        ├── __init__.py
        ├── environment.py
        ├── example.feature
        └── steps
            └── common_steps.py
```

The code for the above can be found [here](https://github.com/donovan-said/python-behave-examples/tree/main/behave/intro-blog-post/features).

### something.feature file

TBC

{% gist cf43ad02e3ca56a87d41cc9afc01c03f %}

### environment.py file

TBC

{% gist c8e66e679195509a1e7bcdf13a000086 %}

### http_step.py file

TBC

{% gist d9591c619f1052982f106b18e1b905b8 %}

## Running your tests

#### behave cli

The behave package comes with a cli tool, which is what's used to execute the tests. There are a bunch of features that
the CLI tool provides, though I won't cover them here, exception for the ```-D``` command, which allows us to provide
additional userdata in the format of key,value pairs. This is how I passed in the env value in the environment.py file.

#### Execution

Executing these tests is very simple. You just need to provide the feature path and any additional flags; in this case
the ```-D``` command to input the environment.

```shell
behave path/to/features -D env=dev
```

#### Output

In the following image, you can see how the feature was executed and the results of the tests.

![Alt text](../img/posts-python-behave-intro-outputs.png)

## Summary

Hopefully, you've gained some insight from this post; it had taken me a while to wrap my head around how all the pieces
tied together, so I wanted to write this down in as simple a format as I could. I aim to follow this up with some more
complex examples. In the meantime, happy coding :raised_hands: