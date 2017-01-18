## Actions

An **Action** is an **Object** that describes discrete piece of work that needs to be done by single a [Actor](/docs/definitions/actors.md).

``Dev: Fix bug``
``QA: Test replication of bug``
``Systems: Upload changeset to staging environment``

An **Action** object contains

- parameters
- dependancies
- description of the action
- reference to Actor

### Action Types

Each Action is given a type Action Types can be created:

``Take Action``, ``Fix Bug``, ``Design Page``, ``Collect Item``.

*Take Action* is a the default generic Action Type which everyone can do.

Action Types enable the system to register a Actor or Group of Actors as being able to take or perform said Action.

The Action Type, ``Fix Bug`` could be created a restriction placed on it so that it can only be given to Developers (a group of Actors grouped by a broad discipline).

**Actions** are scoped to their parent **Issue** and can *Trigger* **Events** outside of their scope. This means that only their parent **Issue** can alter them, or listen to their state, but Actions are able to *Trigger* outside systems.
