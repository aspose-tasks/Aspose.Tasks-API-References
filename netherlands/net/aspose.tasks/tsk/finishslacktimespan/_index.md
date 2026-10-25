---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De duur tussen de vroegste einddatum en de laatste einddatum."
type: docs
weight: 400
url: /nl/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

De duur tussen de vroege einddatum en de late einddatum.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.FinishSlackTimeSpan te lezen. De eigenschap wordt berekend, dus meestal is het niet nodig deze expliciet in te stellen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


