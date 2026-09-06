---
title: "ParseErrorArgs.InvalidValue"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ParseErrorArgs. Obtient la valeur de chaîne qui a déclenché une exception"
type: docs
weight: 40
url: /fr/net/aspose.tasks/parseerrorargs/invalidvalue/
---
## ParseErrorArgs.InvalidValue property

Obtient la valeur de chaîne qui a levé une exception.

```csharp
public string InvalidValue { get; }
```

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

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


