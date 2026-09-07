---
title: "Task.Clone"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Δημιουργεί πλήρη αντίγραφο μιας εργασίας χωρίς υποεργασίες"
type: docs
weight: 1310
url: /el/net/aspose.tasks/task/clone/
---
## Task.Clone method

Δημιουργεί πλήρη αντίγραφο μιας εργασίας χωρίς υποεργασίες.

```csharp
public object Clone()
```

### Τιμή Επιστροφής

Δημιουργήθηκε αντίγραφο μιας εργασίας.

## Παραδείγματα

Εμφανίζει πώς να κλωνοποιήσετε μια εργασία.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


