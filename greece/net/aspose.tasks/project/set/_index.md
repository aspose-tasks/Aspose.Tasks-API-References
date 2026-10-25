---
title: "Project.Set"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το container"
type: docs
weight: 1240
url: /el/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | ο τύπος της αντιστοιχισμένης τιμής. |
| key | το καθορισμένο κλειδί ιδιότητας. [`Prj`](../../prj/) για λήψη του κλειδιού ιδιότητας. |
| val | η τιμή. |

## Παραδείγματα

Δείχνει πώς να ορίσετε τα χαρακτηριστικά της εργασίας.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Αντιστοιχίζει την καθορισμένη ιδιότητα στην καθορισμένη τιμή σε αυτό το δοχείο.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | Key`2 | το καθορισμένο κλειδί ιδιότητας. [`Prj`](../../prj/) για λήψη του κλειδιού ιδιότητας. |
| val | DateTime | η τιμή. |

## Παραδείγματα

Δείχνει πώς να ορίσετε τα χαρακτηριστικά της εργασίας.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


