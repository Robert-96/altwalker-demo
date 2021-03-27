# altwalker-demo

A simple demo using AltWalker. AltWalker is an open source Model-Based Testing framework.

## Setup

Install the python dependencies:

```
$ pip install -r requirements.txt
```

## Running the tests

Check and analyze models for syntax issues:

```
$ altwalker check -m models/default.json "random(vertex_coverage(100))"
```

Verify and analyze the test code for issues (like missing methods or classes):

```
$ altwalker verify tests -m models/default.json
```

Run the tests:

```
$ altwalker online tests -m models/default.json "random(vertex_coverage(100))"
```

Generate a sequence of steps:

```
$ altwalker offline -m models/default.json "random(vertex_coverage(100))" -f steps/steps.json
```

Run the sequence of steps generated with the `offline` command:

```
$ altwalker walk tests steps/steps.json
```
