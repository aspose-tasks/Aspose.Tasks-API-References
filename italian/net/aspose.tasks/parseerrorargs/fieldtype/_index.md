---
title: "ParseErrorArgs.FieldType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ParseErrorArgs. Restituisce il tipo di campo dell'oggetto"
type: docs
weight: 30
url: /it/net/aspose.tasks/parseerrorargs/fieldtype/
---
## ParseErrorArgs.FieldType property

Ottiene il tipo del campo dell'oggetto.

```csharp
public Type FieldType { get; }
```

## Esempi

Mostra come leggere un progetto da uno stream con un file XML contenente caratteri non validi.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // apri il file che contiene XML con intervalli di tempo interrotti
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

### Vedi anche

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


