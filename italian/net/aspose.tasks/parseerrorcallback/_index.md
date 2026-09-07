---
title: "Delegate ParseErrorCallback"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Rappresenta un callback di metodo per gestire gli errori di parsing che possono verificarsi durante la lettura dei dati XML."
type: docs
weight: 1250
url: /it/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

Rappresenta una callback di metodo per gestire gli errori di parsing che possono verificarsi durante la lettura dei dati XML.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mittente | Oggetto | l'oggetto sorgente dell'errore di parsing. |
| args | ParseErrorArgs | l'istanza della classe [`ParseErrorArgs`](../parseerrorargs/) che contiene i dati dell'evento. |

### Valore di ritorno

il valore forzato da impostare sull'oggetto mittente specificato.

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


