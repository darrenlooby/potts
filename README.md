# Potts

Potts Effort Tracker.

We've taken the concepts of [Mechanical Turk](https://en.wikipedia.orgwiki/Amazon_Mechanical_Turk), and [Event Based Applications](https://en.wikipedia.org/wiki/Event-driven_programming), and Graph Data and applied them to the problem of planning and tracking effort.

When a thing needs to be done, the overall effort can be complex. It may involve multiple actions, taken by multiple actors, an those actors might be in different groups or have different roles.

Some of those actors may be human, requiring an interface - and others may be machines, requiring an API.

Moreover, actions might need to be repeated, or skipped, or added after the initial observation that our thing needs to be done.

We create an [Issue](/docs/definitions/issues.md) and allow it to *Listen* out for and *Trigger* [Events](/docs/definitions/events.md).

When an [Event](/docs/definitions/events.md) occurs - those [Issues](/docs/definitions/issues.md) that are *Listening* can change their own [State](/docs/definitions/states.md); such as active or inactive, or who they are assigned to. An [Issues](/docs/definitions/issues.md) that *Triggers* an [Event](/docs/definitions/events.md) can also send [Webhooks](/docs/definitions/webhooks.md) to other [Services](/docs/definitions/services.md). [Event](/docs/definitions/events.md) [Handers](/docs/definitions/handers.md) and incoming [Webhooks](/docs/definitions/webhooks.md) can *Trigger* the creation of new [Issue](/docs/definitions/issues.md) or [Issue Sets](/docs/definitions/issue-sets.md).

Each [Events](/docs/definitions/events.md) that is *Listened* to is *Handled* by an [Event](/docs/definitions/events.md) [Handers](/docs/definitions/handers.md).

## Definitions

### Issues

[Issues](/docs/definitions/issues.md)

[Issue Templates](/docs/definitions/issue-templates.md)

[Issue Sets](/docs/definitions/issue-sets.md)

### States

[States](/docs/definitions/states.md)

### Actions

[Actions](/docs/definitions/actions.md)

[Actors](/docs/definitions/actors.md)

### References

[References](/docs/definitions/references.md)

[Tags](/docs/definitions/tags.md)



### Events

[Events](/docs/definitions/events.md)

[Handlers](/docs/definitions/handlers.md)

### External Interaction

[Webhooks](/docs/definitions/webhooks.md)

[Services](/docs/definitions/services.md)

[Environments](/docs/definitions/environments.md)
