## Event

Events are changes of **State** for some **Issue** or **Service**; or points in **Time**.

This means that an **Event** can be *Triggered* by a new **Issue** being created, an **Issue** being updated, a point in **Time** being reached, an amount of **Time** elapsing, or after having received a message from a **Service**.

### Object Events

Events that are *Triggered* by change in state of Issues or Actions

Used to updated the state of other objects - such as triggering the next action in an issue.

### Service Events

Events that are *Triggered* by Services, or Webhook Responses.

Used to updated the state of other objects - such as triggering the next action in an issue.

### System Events

Changes to parameters that do not trigger a change of state or call to a service - such as Issue Description Updates, or Issue Comment Creation.

Use to send alerts and updates so that a User can be notified of an update to an Issue they are watching.
