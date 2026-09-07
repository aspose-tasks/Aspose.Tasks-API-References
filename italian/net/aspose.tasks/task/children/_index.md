---
title: "Task.Children"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene una raccolta di attività figlie di questo oggetto. Oggetto TaskCollection che rappresenta le attività figlie"
type: docs
weight: 190
url: /it/net/aspose.tasks/task/children/
---
## Task.Children property

Ottiene una collezione di attività figlie di questo oggetto. Oggetto TaskCollection che rappresenta le attività figlie.

```csharp
public TaskCollection Children { get; }
```

## Esempi

Mostra come utilizzare la raccolta di attività per aggiungere un'attività.

```csharp
var project = new Project();

// Aggiungi attività, sottoattività e salva il progetto
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


