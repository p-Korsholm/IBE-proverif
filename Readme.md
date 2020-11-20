
# Formal verification of Accountable Warrant Execution
This repository holds a formal verification of Accountability properties of the Accountable Warrant Execution algorithm.

## How to run verification
To run the verification run the `awe.pv` file using proverif:
```
proverif awe.pv
```

### proving accountability of actors
To prove an actor accountable make all channels that the actor interacts on public(by removing the `[private]`):

```
free SI: channel[private].
free ID: channel[private].
...
free SI: channel.
free ID: channel.
```
