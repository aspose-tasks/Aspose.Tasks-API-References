---
title: "Délégué ParseErrorCallback"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Représente un rappel de méthode pour gérer les erreurs d'analyse qui peuvent survenir lors de la lecture des données XML."
type: docs
weight: 1250
url: /fr/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

Représente un rappel de méthode pour gérer les erreurs d'analyse pouvant survenir lors de la lecture de données XML.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| expéditeur | Objet | l'objet source de l'erreur d'analyse. |
| args | ParseErrorArgs | l'instance de la classe [`ParseErrorArgs`](../parseerrorargs/) qui contient les données de l'événement. |

### Valeur de retour

la valeur coercée à définir pour l'objet expéditeur spécifié.

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


