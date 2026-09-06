---
title: "Énumération CustomPropertyType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Properties.CustomPropertyType énum. Représente une énumération de type de propriété personnalisée"
type: docs
weight: 1560
url: /fr/net/aspose.tasks.properties/custompropertytype/
---
## CustomPropertyType enumeration

Représente une énumération de type de propriété personnalisée.

```csharp
public enum CustomPropertyType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | La propriété n'a aucun type. |
| String | `1` | La propriété est une valeur de chaîne. |
| DateTime | `2` | La propriété est une valeur de date et heure. |
| Number | `3` | La propriété est un nombre entier. |
| Boolean | `4` | La propriété est une valeur booléenne. |

## Exemples

Montre comment travailler avec des collections de propriétés de projet personnalisées.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// ajoutons de nouvelles propriétés personnalisées
// la collection prend en charge les types Boolean, DateTime, Double, String
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// les propriétés personnalisées sont disponibles via la collection typée
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// obtenir la valeur d'une propriété personnalisée
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// itérer sur les noms des propriétés personnalisées
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// on peut supprimer une valeur par clé de chaîne
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// ou on peut effacer complètement la collection
project.CustomProps.Clear();
```

### Voir aussi

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


