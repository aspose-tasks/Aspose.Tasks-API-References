---
title: "Project.RootTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει τη ρίζα του δέντρου των εργασιών"
type: docs
weight: 800
url: /el/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Λαμβάνει τη ρίζα του δέντρου των εργασιών.

```csharp
public Task RootTask { get; }
```

## Παραδείγματα

Δείχνει πώς να προσθέσετε μια εργασία σε ένα έργο χρησιμοποιώντας τη ρίζα της εργασίας του έργου.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


