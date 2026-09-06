---
title: "TableField.TableField"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur TableField. Initialise une nouvelle instance de la classe TableField"
type: docs
weight: 10
url: /fr/net/aspose.tasks/tablefield/tablefield/
---
## TableField constructor

Initialise une nouvelle instance de la classe [`TableField`](../).

```csharp
public TableField()
```

## Exemples

Montre comment lire les tables du projet.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// obtenir la table
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// afficher les informations de tous les champs de la table
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### Voir aussi

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


