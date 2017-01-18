# Potts

Potts effort tracker.

We've taken the concepts of [mechanical turk](https://en.wikipedia.orgwiki/Amazon_Mechanical_Turk), and [event based applications](https://en.wikipedia.org/wiki/Event-driven_programming) and applied them to the problem of planning and tracking effort.

When a thing needs to be done, the overall effort can be complex and involve several people in different teams. Moreover, actions might need to be repeated, or skipped, or added after the initial obervation that our thing needs to be done.

We create an **Issue** and allow it to *Listen* out for and *Trigger* **Events**.

When an **Event** occurs - those **Issues** that are *Listening* can change their own ***State***; such as active or inactive, or who they are assigned to. An **Issue** that *Triggers* an **Event** can also send **Webhooks** to other services. **Event Handlers** and incoming **Webhooks** can *Trigger* the creation of new **Issues** or **Issue Set**.

Each **Event** that is *Listened* to is *Handled* by an **Event Handler**

## Definitions

[Issues](/docs/definitions/issues.md)

[Actions](/docs/definitions/actions.md)

[Actors](/docs/definitions/actors.md)

[Issue Templates](/docs/definitions/issue-templates.md)

[Issue Sets](/docs/definitions/issue-sets.md)

[States](/docs/definitions/states.md)

[Events](/docs/definitions/events.md)

[Handers](/docs/definitions/handers.md)


[Webhooks](/docs/definitions/webhooks.md)

[Services](/docs/definitions/services.md)

[Environments](/docs/definitions/environments.md)
