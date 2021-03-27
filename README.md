# altwalker-demo

A simple demo using AltWalker. AltWalker is an open source Model-Based Testing framework.

## Setup

```
$ pip install -r requirements.txt
```

## Running the tests

```
$ altwalker check -m models/default.json "random(vertex_coverage(100))"
```

```
$ altwalker verify tests -m models/default.json
```

```
$ altwalker online tests -m models/default.json "random(vertex_coverage(100))"
```

```
$ altwalker offline -m models/default.json "random(vertex_coverage(100))" -f steps.json
```

```
$ altwalker walk tests steps.json
```
