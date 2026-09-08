---
title: "Task.ParentProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Taakeigenschap. Haalt het bovenliggende project van een taak op."
type: docs
weight: 930
url: /nl/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Haalt het bovenliggende project van een taak op.

```csharp
public Project ParentProject { get; }
```

## Opmerkingen

Roep Project.UpdateReferences aan om deze eigenschappen bij te werken.

## Voorbeelden

Toont hoe u het bovenliggende project van een taak gebruikt.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// Stel een duur voor de taak in door het standaard projecttijdseenheidtype te gebruiken.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### Zie ook

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


