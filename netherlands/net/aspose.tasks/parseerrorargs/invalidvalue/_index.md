---
title: "ParseErrorArgs.InvalidValue"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ParseErrorArgs property. Haalt de tekenreekswaarde op die een uitzondering veroorzaakte"
type: docs
weight: 40
url: /nl/net/aspose.tasks/parseerrorargs/invalidvalue/
---
## ParseErrorArgs.InvalidValue property

Verkrijgt de tekenreekswaarde die een uitzondering heeft opgegooid.

```csharp
public string InvalidValue { get; }
```

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

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


