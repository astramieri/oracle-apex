# APEX Page Enhancing

The APEX engine primarily relies on two processes to do its job:
- Show Page process, also known as **Page Rendering**
- Accept Page process, also known as **Page Processing**.

## Page Computations

A Page Computation is a logic that can be used to assign values to a single item. 

There are two types of computations:
- **application-level** computations, which are defined at the application level
- **page-level** computations, which are defined at the page level

## Page Processes

A Page Process performs an action at a specified point during the rendering or submission of the page.

## Page Validations

A Page Validation performs a validation on data submitted by the user.

## Dynamics Actions

Dynamic actions provide a way to define complex client-side behavior declaratively without the need for JavaScript.

Creating a Dynamic Action involves specifying:
- when the action happens (with optional conditions)
- when action or actions are performed
- what elements are affected by the action

Dynamic Actions are fired based on events that happen on the page. 

There  are four different categories of events:
- browser events (e.g. *change, click, double-click, etc.*)
- framework events (e.g. *after refresh, before page submit, etc.*)
- component events
- custom events

To debug a dynamic action:
- ensure the application containing the dynamic action has Debugging enabled
- run the page containing the dynamic action
- open the browser's Javascript console
- from the Developer toolbar, click Debug


