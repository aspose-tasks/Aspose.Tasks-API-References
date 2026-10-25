---
title: "Klasse ExtendedAttributeCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ExtendedAttributeCollection klasse. Vertegenwoordigt een verzameling van ExtendedAttribute-objecten"
type: docs
weight: 530
url: /nl/net/aspose.tasks/extendedattributecollection/
---
## ExtendedAttributeCollection class

Vertegenwoordigt een verzameling van [`ExtendedAttribute`](../extendedattribute/) objecten.

```csharp
public class ExtendedAttributeCollection : IList<ExtendedAttribute>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributecollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/extendedattributecollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |
| [Item](../../aspose.tasks/extendedattributecollection/item/) { get; set; } | Haalt op of stelt het element in op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributecollection/add/)(ExtendedAttribute) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/extendedattributecollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/extendedattributecollection/contains/)(ExtendedAttribute) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/extendedattributecollection/copyto/)(ExtendedAttribute[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/extendedattributecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [IndexOf](../../aspose.tasks/extendedattributecollection/indexof/)(ExtendedAttribute) | Bepaalt de index van het opgegeven item in deze collectie. |
| [Insert](../../aspose.tasks/extendedattributecollection/insert/)(int, ExtendedAttribute) | Voegt het opgegeven item in op de opgegeven index. |
| [Remove](../../aspose.tasks/extendedattributecollection/remove/)(ExtendedAttribute) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [RemoveAt](../../aspose.tasks/extendedattributecollection/removeat/)(int) | Verwijdert een item op de opgegeven index. |

## Voorbeelden

Toont hoe je uitgebreide attribuutcollecties gebruikt.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Haal taak met index nul op
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // wis uitgebreide attributen
    task.ExtendedAttributes.Clear();
}

// maak een definitie van een uitgebreid attribuut voor een taak
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// Voeg uitgebreid attribuut 1 toe
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// Voeg uitgebreid attribuut 2 toe
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// werk met uitgebreide attributen...

// verwijder uitgebreid attribuut op index
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// gebruik collectie-indextoegang
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// kopieer attributen naar een ander project
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// verwijder alle definities van uitgebreide attributen
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### Zie ook

* class [ExtendedAttribute](../extendedattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


