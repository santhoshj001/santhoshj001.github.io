---
title: Set Constraints Programattically
tags: [Android, Constraint Layout]
comments: false
description: how to set Constraints Dynamically in Constraint Layout 
---

<br>
Actually, we can programmatically specify the constraints. To do this in a constraint layout, we must first establish a constraintSet that we can clone from a constraint Layout, define the necessary constraints, and then apply to the original constraint layout.
<br>
```java
@PrimaryKey val id: Int
```
<br>
If you need instances of an entity to be uniquely identified by a combination of multiple columns, you can define a composite primary key by listing those columns in the primaryKeys property of @Entity:
<br>
For example :

```java

@Entity(primaryKeys = ["firstName", "lastName"])
data class User(
    val firstName: String?,
    val lastName: String?
)
```

