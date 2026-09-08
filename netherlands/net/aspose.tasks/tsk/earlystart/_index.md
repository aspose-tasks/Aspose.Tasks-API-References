---
title: "Tsk.EarlyStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De vroegste datum waarop een taak mogelijk kan beginnen, gebaseerd op de vroegste startdatums van voorganger- en opvolgtaken en andere beperkingen."
type: docs
weight: 340
url: /nl/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

De vroegste datum waarop een taak mogelijk kan beginnen, gebaseerd op vroege startdatums van voorganger- en opvolgtaak en andere beperkingen.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.EarlyStart te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


