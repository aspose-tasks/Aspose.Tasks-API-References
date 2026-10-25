---
title: "Tsk.IgnoreWarnings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Indica se nascondere l'indicatore di avviso di conflitto di programmazione in Microsoft Project"
type: docs
weight: 540
url: /it/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Indica se nascondere l'indicatore di avviso di conflitto di programmazione in Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IgnoreWarnings.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


