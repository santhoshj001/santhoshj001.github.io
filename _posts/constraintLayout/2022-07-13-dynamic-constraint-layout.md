---
title: Set Constraints Programattically
tags: [Android, Constraint Layout]
comments: false
description: how to set Constraints Dynamically in Constraint Layout 
---

<br><br><br>
Actually, we can programmatically specify the constraints. To do this in a constraint layout, we must first establish a constraintSet that we can clone from a constraint Layout, define the necessary constraints, and then apply to the original constraint layout.
<br>
```java
    val layout = binding.mConstraintLayout
    var constraintSet = ConstraintSet()
    constraintSet.clone(layout)
```
<br>
Once created the ConstaintSet we can set the contraints like the example 
here we are defining the constraint betweeen button1 and button2 
<br>
```java
constraintSet.connect(button1.id, ConstraintSet.BOTTOM, button2.id, ConstraintSet.TOP)
```

