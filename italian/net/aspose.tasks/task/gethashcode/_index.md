---
title: "Task.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo di Task. Restituisce un valore di codice hash per questo Task"
type: docs
weight: 1350
url: /it/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Restituisce un valore di codice hash per questa Task.

```csharp
public override int GetHashCode()
```

### Valore di ritorno

restituisce un valore di hash per questo oggetto.

## Esempi

Mostra come ottenere un codice hash di un'attività.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// Il codice hash di un'attività è basato sull'uid e sul nome dell'attività
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


