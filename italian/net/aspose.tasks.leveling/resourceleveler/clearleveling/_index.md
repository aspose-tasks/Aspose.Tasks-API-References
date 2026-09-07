---
title: "ResourceLeveler.ClearLeveling"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceLeveler. Cancella qualsiasi ritardo di livellamento precedentemente aggiunto al progetto durante il livellamento delle risorse."
type: docs
weight: 10
url: /it/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Cancella qualsiasi ritardo di livellamento precedentemente aggiunto al progetto durante il livellamento delle risorse.

```csharp
public static void ClearLeveling(Project project)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| progetto | Project | Progetto per cancellare il livellamento. |

## Esempi

Mostra come livellare tutte le risorse del progetto utilizzando le opzioni predefinite.

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

### Vedi anche

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Cancella qualsiasi ritardo di livellamento precedentemente aggiunto alle attività specificate durante il livellamento delle risorse.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| attività | IEnumerable`1 | L'enumerabile contenente le attività per le quali il ritardo di livellamento deve essere cancellato. |

### Vedi anche

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


