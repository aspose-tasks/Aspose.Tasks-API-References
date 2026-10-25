---
title: "Table.ShowAddNewColumn"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Table. Obtient ou définit une valeur indiquant s'il faut afficher l'interface Add New Column. Pris en charge à partir de la version MSP 2010 et suivantes"
type: docs
weight: 70
url: /fr/net/aspose.tasks/table/showaddnewcolumn/
---
## Table.ShowAddNewColumn property

Obtient ou définit une valeur indiquant s'il faut afficher l'interface 'Add New Column'. Pris en charge à partir de la version MSP 2010 et suivantes.

```csharp
public bool ShowAddNewColumn { get; set; }
```

## Exemples

Montre comment définir une nouvelle table (utilisée pour les vues).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// obtenir une table à modifier
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// ajuster certaines propriétés
// définit une valeur indiquant si la hauteur de la ligne d'en-tête de la table peut être ajustée
table.AdjustHeaderRowHeight = true;

// définit le format de date de la table.
table.DateFormat = DateFormat.DateDdMmYyyy;

// définit une valeur indiquant si la première colonne d'une table est verrouillée ou modifiable
table.LockFirstColumn = true;

// définit la hauteur de ligne dans une table, où la hauteur de ligne correspond au nombre de lignes de texte
table.RowHeight = 10;

// définit une valeur indiquant s'il faut afficher l'interface « Ajouter une nouvelle colonne »
table.ShowAddNewColumn = true;

// définit une valeur indiquant si le projet affiche le nom de la table dans la liste déroulante Tables de l'onglet Affichage du ruban
table.ShowInMenu = true;

// permet d'enregistrer la table mise à jour
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


