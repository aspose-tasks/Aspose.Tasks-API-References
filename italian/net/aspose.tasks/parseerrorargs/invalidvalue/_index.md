---
title: "ParseErrorArgs.InvalidValue"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ParseErrorArgs. Restituisce il valore stringa che ha generato un'eccezione"
type: docs
weight: 40
url: /it/net/aspose.tasks/parseerrorargs/invalidvalue/
---
## ParseErrorArgs.InvalidValue property

Ottiene il valore stringa che ha generato un'eccezione.

```csharp
public string InvalidValue { get; }
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


