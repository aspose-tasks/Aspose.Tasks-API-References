---
title: "Tsk.DisplayAsSummary"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of de taak moet worden weergegeven als een samenvattingstaak. Alleen lezen ondersteund voor XML-formaat."
type: docs
weight: 280
url: /nl/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Bepaalt of de taak moet worden weergegeven als een samenvattende taak. Alleen lezen ondersteund voor XML-indeling.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.DisplayAsSummary te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


