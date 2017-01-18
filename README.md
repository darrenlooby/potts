# Potts

Potts effort tracker.

We've taken the concepts of [mechanical turk](https://en.wikipedia.orgwiki/Amazon_Mechanical_Turk), and [event based applications](https://en.wikipedia.org/wiki/Event-driven_programming) and applied them to the problem of planning and tracking effort.

When a thing needs to be done, the overall effort can be complex and involve several people in different teams. Moreover, actions might need to be repeated, or skipped, or added after the initial obervation that our thing needs to be done.

We create an **Issue** and allow it to *Listen* out for and *Trigger* **Events**.

When an **Event** occurs - those **Issues** that are *Listening* can change their own ***State***; such as active or inactive, or who they are assigned to. An **Issue** that *Triggers* an **Event** can also send **Webhooks** to other services. **Event Handlers** and incoming **Webhooks** can *Trigger* the creation of new **Issues** or **Issue Set**.

Each **Event** that is *Listened* to is *Handled* by an **Event Handler**

## Definitions

[Issues](/blankbox/potts/blob/master/docs/issues.md)

[Actions](/blankbox/potts/blob/master/docs/actions.md)

## Actors

An **Actor** is person or machine that can perform an **Action**.

## Issue Template

An **Issue Template** is a collection of predefined **Actions** and **References**, and default **State**.

## Issue Set

An **Issue Set** is a collection of **Issue Templates** that can be applied in a single process.

## State

A **State** is a collection of parameters for an object that can be *Listened* to. Some parameters do not *Trigger* **Events** - such as references. Creating or updating a **Reference** for an **Issue** does not *Trigger* an **Event**.

## Event

Events are changes of **State** for some **Issue** or **Service**; or points in **Time**.

This means that an **Event** can be *Triggered* by a new **Issue** being created, an **Issue** being updated or changed, a point in **Time** being reached, an amout of **Time** elapsing, or after having recieved a message from a **Service**.

## Handlers

**Events** are *Handled* logically. When an **Event** occurs, it *Triggers* one or more **Event Handlers** who each determine an outcome. They do this by assising the properties of their Object - which can be an **Issue**, **Environment**, or **Service**.

A **Handler** has access to the *Trigger* object - for exmaple, the **Issue** whose ***State*** changed, or the message sent by a **Service**. Certain **Handlers** also have access to other **Isssues** and / or the ability to *Trigger* **Webhooks**.

## Webhooks

## Service

## Environments

**Time** is a special case of **Environment**, which is managed internally. **Environments** are treated like sensor data - and can data regarding the machine or server being used or a client application.
