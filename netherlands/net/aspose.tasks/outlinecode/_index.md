---
title: "Klasse OutlineCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineCode class. Vertegenwoordigt een waarde van een outlinecode"
type: docs
weight: 1150
url: /nl/net/aspose.tasks/outlinecode/
---
## OutlineCode class

Stelt een waarde van een outline‑code voor.

```csharp
public class OutlineCode
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | Initialiseert een nieuw exemplaar van de `OutlineCode` class. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Initialiseert een nieuw exemplaar van de `OutlineCode` class met de opgegeven Outline Code en een van zijn waarden. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Haalt op of stelt de numerieke waarde van het aangepaste veld project Id in. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Haalt op of stelt de GUID van de waarde in de waardelijst in. De ValueGuid komt overeen met de FieldGuid in de waardelijst. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Haalt op of stelt de Id in de waardelijst in die gekoppeld is aan de definitie in de outline‑code‑collectie. |

## Opmerkingen

Twee gegevensstukken zijn nodig - een verwijzing naar de outline‑codetabel die gespecificeerd wordt door de FieldId, en de waarde die gespecificeerd wordt door ofwel de ValueId of de ValueGuid‑verwijzing naar de waardelijst.

## Voorbeelden

Toont hoe de outline‑codes van een taak gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// outline‑codes lezen
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


