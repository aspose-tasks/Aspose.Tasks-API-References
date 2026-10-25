---
title: "Tsk.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η διάρκεια κατά την οποία η πραγματική υπερωριακή εργασία προστατεύεται."
type: docs
weight: 70
url: /el/net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

Η διάρκεια κατά την οποία η πραγματική υπερωριακή εργασία προστατεύεται.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


