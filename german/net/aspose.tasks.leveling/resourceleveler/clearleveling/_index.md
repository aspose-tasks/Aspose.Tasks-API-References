---
title: "ResourceLeveler.ClearLeveling"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ResourceLeveler-Methode. Löscht jede Ebenungsverzögerung, die dem Projekt während der Ressourcenebene zuvor hinzugefügt wurde."
type: docs
weight: 10
url: /de/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Löscht jede Leveling-Verzögerung, die dem Projekt während des Ressourcen-Levelings zuvor hinzugefügt wurde.

```csharp
public static void ClearLeveling(Project project)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Projekt | Projekt | Projekt, um die Ebenung zu löschen. |

## Beispiele

Zeigt, wie alle Ressourcen des Projekts mit den Standardoptionen gelevelt werden.

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

### Siehe auch

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Löscht jede Leveling-Verzögerung, die den angegebenen Aufgaben während des Ressourcen-Levelings zuvor hinzugefügt wurde.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Aufgaben | IEnumerable`1 | Die Aufzählung, die Aufgaben enthält, für die die Ebenungsverzögerung gelöscht werden soll. |

### Siehe auch

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


