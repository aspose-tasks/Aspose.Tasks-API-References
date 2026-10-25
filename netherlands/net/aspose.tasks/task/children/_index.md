---
title: "Task.Children"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task eigenschap. Haalt een verzameling van onderliggende taken van dit object op. TaskCollection object dat kindtaken vertegenwoordigt"
type: docs
weight: 190
url: /nl/net/aspose.tasks/task/children/
---
## Task.Children property

Haalt een collectie van onderliggende taken van dit object op. TaskCollection-object dat onderliggende taken vertegenwoordigt.

```csharp
public TaskCollection Children { get; }
```

## Voorbeelden

Toont hoe een takenverzameling gebruikt wordt om een taak toe te voegen.

```csharp
var project = new Project();

// Taak, subtaak toevoegen en project opslaan
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


