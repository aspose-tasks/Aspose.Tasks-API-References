---
title: "Project.CriticalPath"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project eigenschap. Haalt een collectie op die een lijst bevat van kritieke taken die het kritieke pad van dit project vormen. Dit is een On‑operatie waarbij n het aantal taken in het project is."
type: docs
weight: 180
url: /nl/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Haalt een collectie op die een lijst bevat van kritieke taken die het kritieke pad van dit project vormen. Dit is een O(n)-operatie, waarbij n het aantal taken in het project is.

```csharp
public TaskCollection CriticalPath { get; }
```

### Retourwaarde

een collectie die een lijst van alle kritieke taken weergeeft.

## Voorbeelden

Toont hoe het kritieke pad van het project berekend kan worden.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Toon nu het kritieke pad
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### Zie ook

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


