## Event

Events are changes of [**State**](/docs/definitions/states.md) for some [**Issue**](/docs/definitions/issues.md) or [**Service**](/docs/definitions/services.md); or points in **Time**.

This means that an **Event** can be *Triggered* by a new **Issue** being created, an **Issue** being updated, a point in **Time** being reached, an amount of **Time** elapsing, or by having received a message from a **Service**.

### Object Events

Events that are *Triggered* by change in state of Issues or [**Actions**](/docs/definitions/actions.md)

Used to updated the state of other objects - such as triggering the next action in an Issue.

### Service Events

Events that are *Triggered* by Services, or [**WebHooks**](/docs/definitions/webhooks.md) Responses.

Used to updated the state of other objects - such as triggering the next action in an Issue.

### System Events

Changes to parameters that do not trigger a change of state or call to a service - such as Issue Description Updates, or Issue Comment Creation.

Use to send alerts and updates so that a User can be notified of an update to an Issue they are watching - without triggering a sequence of events.
