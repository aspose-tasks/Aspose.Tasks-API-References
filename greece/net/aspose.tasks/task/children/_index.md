---
title: "Task.Children"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει μια συλλογή παιδικών εργασιών αυτού του αντικειμένου. Αντικείμενο TaskCollection που αντιπροσωπεύει εργασίες παιδιών"
type: docs
weight: 190
url: /el/net/aspose.tasks/task/children/
---
## Task.Children property

Λαμβάνει μια συλλογή παιδικών εργασιών αυτού του αντικειμένου. Αντικείμενο TaskCollection που αντιπροσωπεύει παιδικές εργασίες.

```csharp
public TaskCollection Children { get; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη συλλογή εργασιών για να προσθέσετε μια εργασία.

```csharp
var project = new Project();

// Προσθέστε εργασία, υποεργασία και αποθηκεύστε το έργο
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


