---
title: "TaskUtils.TaskChildrenCount"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskUtils methode. Rekent recursief het aantal kindtaken van taken over alle niveaus"
type: docs
weight: 40
url: /nl/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Berekent recursief het aantal onderliggende taken van een taak over alle niveaus.

```csharp
public static int TaskChildrenCount(Task task)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taak | Taak | De taak waarvan de kinderen worden berekend. |

### Retourwaarde

Het aantal kinderen.

## Voorbeelden

Toont hoe de &lt;see cref=\"Aspose.Tasks.Util.TaskUtils.TaskChildrenCount\" /&gt; methode te gebruiken.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// berekent recursief het aantal kindtaken van een taak over alle niveaus
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### Zie ook

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


