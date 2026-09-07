---
title: "Project.RootTask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Restituisce la radice dell'albero delle attività"
type: docs
weight: 800
url: /it/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Ottiene la radice dell'albero delle attività.

```csharp
public Task RootTask { get; }
```

## Esempi

Mostra come aggiungere un'attività in un progetto utilizzando l'attività radice del progetto.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


