---
title: "Delegate ParseErrorCallback"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Stelt een method callback voor om parse-fouten af te handelen die kunnen optreden bij het lezen van xml-gegevens."
type: docs
weight: 1250
url: /nl/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

Stelt een methode‑callback voor om parse‑fouten af te handelen die kunnen optreden bij het lezen van xml‑gegevens.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| zender | Object | het bronobject van de parse-fout. |
| args | ParseErrorArgs | de instantie van de [`ParseErrorArgs`](../parseerrorargs/) klasse die de gebeurtenisgegevens bevat. |

### Retourwaarde

de omgezette waarde die moet worden ingesteld op het opgegeven zenderobject.

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


