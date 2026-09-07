---
title: "Task.Clone"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Crea una copia completa di un task senza sottotask"
type: docs
weight: 1310
url: /it/net/aspose.tasks/task/clone/
---
## Task.Clone method

Crea una copia completa di un'attività senza sottoattività.

```csharp
public object Clone()
```

### Valore di ritorno

Creata copia di un'attività.

## Esempi

Mostra come clonare un'attività.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


