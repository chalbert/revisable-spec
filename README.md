# Revisable Spec

Defines an interface that JavaScript objects can implement to handle revisions.

## Spec

- The `rev` Global Symbol property MUST specify the current revision of an object.
- The `rev` Global Symbol property MAY be `null` if no revision exist.
- The current state of the object MAY be different to the last commmited value. For example, committing could be throttled, or only done when the changes are deemed valid.
- 

## Global Symbols

| Symbol name | Description |
| --- | --- |
| rev | The current revision. |
| maxRev | The maximum number of revisions to keep. Optional. If absent, maximum will be `0`  |
| commit | Method that creates a new revision. To use when an object value changes. |
| revert | Method that reverts the object to its latest revision. |
| revs | Holds the list of an object revision. |

## Interface

### commit(newValue)

## Type

### Rev

