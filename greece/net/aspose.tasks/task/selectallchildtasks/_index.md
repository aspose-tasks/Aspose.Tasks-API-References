---
title: "Task.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Συλλέγει αναδρομικά όλες τις θυγατρικές εργασίες αυτής της εργασίας"
type: docs
weight: 1400
url: /el/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Συλλέγει αναδρομικά όλες τις θυγατρικές εργασίες αυτής της εργασίας.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Τιμή Επιστροφής

Μια λίστα με τις θυγατρικές εργασίες αυτής της εργασίας.

## Παραδείγματα

Δείχνει πώς να επαναλάβετε τις θυγατρικές εργασίες.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


