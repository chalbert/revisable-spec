# Revisable Spec

Defines an interface that JavaScript objects can implement to handle revisions.

## Spec

- The `rev` Global Symbol property WILL specify the current revision of an object.
- The `rev` Global Symbol property MAY be null if no revision exist.
- The `commit` Global Symbol property MAY be null if no revision exist.

## Global Symbols

| Symbol name | Description |
| --- | --- |
| rev | The current revision |
| commit | Method that creates a new revision. To use when an object value changes. |
| revs | Holds the list of an object revision |

## Interface

### commit(newValue)

## Type

### Rev

