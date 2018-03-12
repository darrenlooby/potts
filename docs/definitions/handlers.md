## Handlers

**Events** are *Handled* logically. When an **Event** occurs, it *Triggers* one or more **Event Handlers** who each determine an outcome. They do this by assessing the properties of their Object - which can be an **Issue**, **Environment**, or **Service**.

A **Handler** has access to the *Trigger* object - for example, the **Issue** whose ***State*** changed, or the message sent by a **Service**. Certain **Handlers** also have access to other **Issues** and / or the ability to *Trigger* **Webhooks**.
