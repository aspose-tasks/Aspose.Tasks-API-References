---
title: "Tsk.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De duur gedurende welke daadwerkelijk werk beschermd is. Lezen wordt alleen ondersteund voor XML-formaat."
type: docs
weight: 100
url: /nl/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

De duur gedurende welke feitelijk werk wordt beschermd. Lezen wordt alleen ondersteund voor XML-indeling.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.ActualWorkProtected te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


