---
title: "Project.RootTask"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-eigenschap. Haalt de wortel van de taakboom op"
type: docs
weight: 800
url: /nl/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Haalt de root van de taakboom op.

```csharp
public Task RootTask { get; }
```

## Voorbeelden

Toont hoe een taak aan een project toe te voegen door de rootprojecttaak te gebruiken.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


