---
title: "Tsk.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η διάρκεια κατά την οποία η πραγματική εργασία προστατεύεται. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML"
type: docs
weight: 100
url: /el/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

Η διάρκεια κατά την οποία η πραγματική εργασία προστατεύεται. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


