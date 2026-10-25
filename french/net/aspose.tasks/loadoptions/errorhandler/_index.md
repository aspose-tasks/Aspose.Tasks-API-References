---
title: "LoadOptions.ErrorHandler"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "LoadOptions propriété. Obtient ou définit une méthode de rappel pour gérer les erreurs d'analyse xml"
type: docs
weight: 40
url: /fr/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

Obtient ou définit une méthode de rappel pour gérer les erreurs d'analyse XML.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Exemples

Montre comment lire un projet à partir d'un fichier XML Primavera avec une erreur d'analyse.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// Renvoie le projet avec un UID spécial
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Montre comment charger un projet Primavera en utilisant &lt;see cref=\"LoadOptions\" /&gt; avec gestion des erreurs.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // définir les options de lecture primavera
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // travailler avec le projet...
}

private static object CustomDurationHandlerForFile(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var value = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", value);
    return value;
}
```

### Voir aussi

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


