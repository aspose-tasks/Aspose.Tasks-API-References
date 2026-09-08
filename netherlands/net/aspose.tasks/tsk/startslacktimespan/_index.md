---
title: "Tsk.StartSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De duur tussen de vroegste start- en laatste startdatums"
type: docs
weight: 1020
url: /nl/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

De duur tussen de Early Start- en Late Start-datums.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.StartSlackTimeSpan te lezen. De eigenschap wordt berekend, dus meestal is het niet nodig deze expliciet in te stellen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


