---
title: "Classe ParseErrorArgs"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ParseErrorArgs. Fournit des données pour le délégué ParseErrorCallback."
type: docs
weight: 1240
url: /fr/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

Fournit des données pour le délégué [`ParseErrorCallback`](../parseerrorcallback/).

```csharp
public class ParseErrorArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | Obtient l'exception levée lors de l'analyse de la valeur de chaîne. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | Obtient le nom du champ d'objet. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | Obtient le type du champ d'objet. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | Obtient la valeur de chaîne qui a levé une exception. |

## Exemples

Montre comment lire un projet à partir d'un flux avec un fichier XML contenant des caractères invalides.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // ouvrir le fichier qui contient du XML avec des intervalles de temps corrompus
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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


