---
title: "Task.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτήν την εργασία"
type: docs
weight: 1350
url: /el/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτήν την Task.

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να λάβετε έναν κώδικα κατακερματισμού μιας εργασίας.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// ο κωδικός κατακερματισμού μιας εργασίας βασίζεται στο uid και το όνομα της εργασίας
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


