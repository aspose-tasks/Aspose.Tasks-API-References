---
title: "ResourceLeveler.ClearLeveling"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceLeveler method. Verwijdert elke leveling-vertraging die eerder aan het project is toegevoegd tijdens resource-leveling."
type: docs
weight: 10
url: /nl/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Verwijdert elke nivelleringsvertraging die eerder aan het project is toegevoegd tijdens resource‑nivellering.

```csharp
public static void ClearLeveling(Project project)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Project om leveling te verwijderen. |

## Voorbeelden

Toont hoe alle resources van een project te nivelleren met standaardopties.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### Zie ook

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Verwijdert elke nivelleringsvertraging die eerder aan de opgegeven taken is toegevoegd tijdens resource‑nivellering.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taken | IEnumerable`1 | De enumerable die taken bevat waarvoor de leveling-vertraging moet worden verwijderd. |

### Zie ook

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


