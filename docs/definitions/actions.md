## Actions

An *Action* is a decrete piece of work that needs to be done by single **Actor**.

``Dev: Fix bug``
``QA: Test replication of bug``
``Systems: Upload changeset to staging environment``
 
An **Action** object contains

- parameters
- dependancies
- description of the action
- reference to Actor

**Actions** are scoped to their parent **Issue** and can *Trigger* **Events** outside of their scope. This means that only their parent **Issue** can alter them, or listen to their state.
