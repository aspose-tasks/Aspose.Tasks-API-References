---
title: "Classe ParseErrorArgs"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ParseErrorArgs. Fornisce dati per il delegato ParseErrorCallback"
type: docs
weight: 1240
url: /it/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

Fornisce dati per il delegato [`ParseErrorCallback`](../parseerrorcallback/).

```csharp
public class ParseErrorArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | Ottiene l'eccezione generata durante l'analisi del valore stringa. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | Ottiene il nome del campo dell'oggetto. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | Ottiene il tipo del campo dell'oggetto. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | Ottiene il valore stringa che ha generato un'eccezione. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


