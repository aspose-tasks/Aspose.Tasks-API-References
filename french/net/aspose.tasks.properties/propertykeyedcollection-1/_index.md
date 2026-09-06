---
title: "Classe PropertyKeyedCollectionT"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Properties.PropertyKeyedCollection1T classe. Une classe de base d'une collection de propriétés"
type: docs
weight: 1600
url: /fr/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

Une classe de base d'une collection de propriétés.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| Paramètre | Description |
| --- | --- |
| T | Le type de propriété. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | Obtient le nombre de propriétés dans la collection. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | Obtient la Property associée à la clé spécifiée. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | Obtient la collection de tous les noms de propriétés. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | Crée une nouvelle propriété personnalisée. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | Détermine si le [`PropertyCollection`](../propertycollection-1/) contient une propriété avec le nom spécifié. |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


