---
title: "Task.Successors"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει ένα αντικείμενο TaskCollection που περιέχει όλους τους διαδόχους αυτού του αντικειμένου Task"
type: docs
weight: 1200
url: /el/net/aspose.tasks/task/successors/
---
## Task.Successors property

Λαμβάνει ένα αντικείμενο [`TaskCollection`](../../taskcollection/) που περιέχει όλους τους διαδόχους αυτού του αντικειμένου Task.

```csharp
public TaskCollection Successors { get; }
```

### Τιμή Επιστροφής

Αντικείμενο μόνο για ανάγνωση της κλάσης [`TaskCollection`](../../taskcollection/).

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους διαδόχους του task.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### Δείτε επίσης

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


