---
title: "Task.TimephasedData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task-eigenschap. Haalt een TimephasedDataCollection-object op of stelt dit in voor deze taak. Het tijdgephaseerde datablock dat aan een taak is gekoppeld"
type: docs
weight: 1220
url: /nl/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Haalt een TimephasedDataCollection-object op van deze taak. Het tijdsfasegegevensblok dat aan een taak is gekoppeld.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Opmerkingen

Lezen wordt alleen ondersteund voor XML-indeling.

## Voorbeelden

Toont hoe je over de tijdgephaseerde gegevens van een taak iterereert.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


