---
title: "Task.Predecessors"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει ένα αντικείμενο TaskCollection που περιέχει όλους τους προκάτοχους αυτού του αντικειμένου Task"
type: docs
weight: 980
url: /el/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Λαμβάνει ένα αντικείμενο [`TaskCollection`](../../taskcollection/) που περιέχει όλους τους προκάτοχους αυτού του αντικειμένου Task.

```csharp
public TaskCollection Predecessors { get; }
```

### Τιμή Επιστροφής

Αντικείμενο μόνο για ανάγνωση της κλάσης [`TaskCollection`](../../taskcollection/).

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους προκάτοχους μιας εργασίας.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### Δείτε επίσης

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


