---
title: "Klasse OutlineCodeCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineCodeCollection klasse. Vertegenwoordigt een collectie van OutlineCode-objecten"
type: docs
weight: 1160
url: /nl/net/aspose.tasks/outlinecodecollection/
---
## OutlineCodeCollection class

Vertegenwoordigt een collectie van [`OutlineCode`](../outlinecode/) objecten.

```csharp
public class OutlineCodeCollection : IList<OutlineCode>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodecollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/outlinecodecollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |
| [Item](../../aspose.tasks/outlinecodecollection/item/) { get; set; } | Retourneert of stelt het element in op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodecollection/add/)(OutlineCode) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/outlinecodecollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/outlinecodecollection/contains/)(OutlineCode) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/outlinecodecollection/copyto/)(OutlineCode[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/outlinecodecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [IndexOf](../../aspose.tasks/outlinecodecollection/indexof/)(OutlineCode) | Bepaalt de index van het opgegeven item in deze collectie. |
| [Insert](../../aspose.tasks/outlinecodecollection/insert/)(int, OutlineCode) | Voegt het opgegeven item in op de opgegeven index. |
| [Remove](../../aspose.tasks/outlinecodecollection/remove/)(OutlineCode) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [RemoveAt](../../aspose.tasks/outlinecodecollection/removeat/)(int) | Verwijdert een item op de opgegeven index. |

## Voorbeelden

Toont hoe je met outline code-collecties kunt werken.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

for (var i = 0; i < collector.Tasks.Count; i++)
{
    var current = collector.Tasks[i];
    if (current.Get(Tsk.Id) == 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes for the " + current.Get(Tsk.Name) + " task.");
    Console.WriteLine("Count of outline codes: " + current.OutlineCodes.Count);
    foreach (var outlineCode in current.OutlineCodes)
    {
        Console.WriteLine("Field Id: " + outlineCode.FieldId);
        Console.WriteLine("Value Id: " + outlineCode.ValueId);
        Console.WriteLine("Value Guid: " + outlineCode.ValueGuid);
        Console.WriteLine();
    }
}

// voeg een aangepaste outline code-definitie toe
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// maak outline code
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// men kan controleren dat de collectie niet alleen-lezen is.
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// voeg code met 2 in een verkeerde positie in.
task.OutlineCodes.Insert(0, code2);

// repareer het
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// voeg code met 2 in een juiste positie in.
task.OutlineCodes.Insert(2, code2);

// controleer dat de code is ingevoegd.
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// werken met outline codes
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// voeg een aangepaste outline code-definitie toe
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// maak outline code
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// werken met outline codes
// ...

// verwijder outline code
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// wis alle waarden in één keer.
task.OutlineCodes.Clear();
```

### Zie ook

* class [OutlineCode](../outlinecode/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


