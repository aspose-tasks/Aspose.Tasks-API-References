---
title: "Classe Value"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Value. Représente une valeur dans une liste de valeurs"
type: docs
weight: 2800
url: /fr/net/aspose.tasks/value/
---
## Value class

Représente une valeur dans une liste de valeurs.

```csharp
public class Value
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Value](value/)() | Initialise une nouvelle instance de la classe `Value`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | Obtient ou définit la valeur réelle si elle peut être représentée comme DateTime. La valeur par défaut est MinValue. |
| [Description](../../aspose.tasks/value/description/) { get; set; } | Obtient ou définit la description d'une valeur. |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | Obtient ou définit la valeur réelle utilisée pour représenter la durée. |
| [Id](../../aspose.tasks/value/id/) { get; set; } | Obtient ou définit l'identifiant unique d'une valeur dans un projet. |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | Obtient ou définit la valeur réelle utilisée pour représenter un nombre ou une valeur de coût. |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | Obtient ou définit les informations phonétiques concernant le nom du champ personnalisé. |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | Obtient ou définit la valeur réelle utilisée pour représenter une chaîne de texte. |
| [Val](../../aspose.tasks/value/val/) { get; set; } | Obtient ou définit la valeur réelle dans la représentation interne. Privilégiez l'utilisation des propriétés fortement typées listées ci-dessous. |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | Obtient un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet. |

## Exemples

Montre comment lire le travail avec des valeurs de recherche.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Créer une définition d'attribut étendu de type texte
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Ajouter des valeurs de recherche pour la définition d'attribut étendu
textLookup.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1", Phonetic = "Town One" });
textLookup.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2", Phonetic = "Town Two" });

Console.WriteLine("Iterate over text lookup values:");
foreach (var value in textLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("String Value: " + value.StringValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Créer une définition d'attribut étendu de type durée
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// Ajouter des valeurs de recherche pour la définition d'attribut étendu
durationLookup.AddLookupValue(new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours", Phonetic = "Four hours" });
durationLookup.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(8, TimeUnitType.Hour), Description = "1 day", Phonetic = "One day" });
durationLookup.AddLookupValue(new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour", Phonetic = "One hour" });
durationLookup.AddLookupValue(new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days", Phonetic = "Ten days" });

Console.WriteLine("Iterate over duration lookup values:");
foreach (var value in durationLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Duration: " + value.Duration);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Créer une définition d'attribut étendu de type date
var dateLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Date,
    ExtendedAttributeTask.Date1,
    "Custom Date");
dateLookup.AddLookupValue(new Value { Id = 7, DateTimeValue = new DateTime(2020, 4, 27, 8, 0, 0), Description = "Start Date", Phonetic = "Start Date" });

Console.WriteLine("Iterate over date lookup values:");
foreach (var value in dateLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("DateTime Value: " + value.DateTimeValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Créer une définition d'attribut étendu de type nombre
var numericLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Number,
    ExtendedAttributeTask.Number1,
    "Number of tons");
numericLookup.AddLookupValue(new Value { Id = 8, NumericValue = 10, Description = "10 tons", Phonetic = "Ten tons" });
numericLookup.AddLookupValue(new Value { Id = 9, NumericValue = 20, Description = "20 tons", Phonetic = "Twenty tons" });
numericLookup.AddLookupValue(new Value { Id = 10, NumericValue = 30, Description = "30 tons", Phonetic = "Thirty tons" });

Console.WriteLine("Iterate over numeric lookup values:");
foreach (var value in numericLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Numeric Value: " + value.NumericValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

project.ExtendedAttributes.Add(textLookup);
project.ExtendedAttributes.Add(durationLookup);
project.ExtendedAttributes.Add(dateLookup);
project.ExtendedAttributes.Add(numericLookup);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


