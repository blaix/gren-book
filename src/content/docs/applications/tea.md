---
title: The Elm Architecture
description: Gren follows The Elm Architecture, sometimes called Model/View/Update (MVU).
---

Gren applications follow [The Elm Architecture](https://guide.elm-lang.org/architecture/).

_Instead of the consider talking about the entire application as a pure function: (event, state) => state_
_Then if you need to perform effects: (event, state) => (state, effects[])_
_The effects are values representing the effect you want the runtime to perform._

There are three main concepts with this type of architecture:

* **Model**: Holds your application state. "Application state" is the runtime data your application cares about. For example, the current logged in user might be part of your model.
* **View**: Renders the UI for your application state. This might be an HTML page, a JSON response, or some text on the command line.
* **Update**: Modifies your application state in response to events. Maybe a user clicked logout, so you return a new model with the user removed.

As your application runs, the path through the architecture looks like this:

```mermaid
flowchart LR
  initial[Initial Model] --> View
  View --> Update
  Update --> new[New Model]
  new --> View
```

If you want to jump straight into... TODO

The next sections will go into detail... TODO

## Model

TODO

## Update

TODO

## View

TODO
