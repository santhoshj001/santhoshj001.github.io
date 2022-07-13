---
title: Set Constraints Programattically
tags: [Android, Constraint Layout]
comments: false
description: how to set Constraints Dynamically in Constraint Layout 
---

<br>

Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table. The most straightforward way of doing this is to annotate a single column with @PrimaryKey:
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

