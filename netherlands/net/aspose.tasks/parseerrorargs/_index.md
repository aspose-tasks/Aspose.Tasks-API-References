---
title: "Klasse ParseErrorArgs"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ParseErrorArgs klasse. Biedt gegevens voor de ParseErrorCallback delegate"
type: docs
weight: 1240
url: /nl/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

Biedt gegevens voor de [`ParseErrorCallback`](../parseerrorcallback/) delegate.

```csharp
public class ParseErrorArgs
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | Verkrijgt de opgegooide uitzondering tijdens het parseren van de tekenreekswaarde. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | Verkrijgt de naam van het objectveld. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | Verkrijgt het type van het objectveld. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | Verkrijgt de tekenreekswaarde die een uitzondering heeft opgegooid. |

## Voorbeelden

Toont hoe een project te lezen vanuit een stream met een XML‑bestand met ongeldige tekens.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // open het bestand dat XML met gebroken tijdsintervallen bevat
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


