---
title: "Classe Table"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Table. Représente un tableau dans Project."
type: docs
weight: 2320
url: /fr/net/aspose.tasks/table/
---
## Table class

Représente une table dans Project

```csharp
public class Table
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Table](table/)() | Initialise une nouvelle instance de la classe `Table`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Obtient ou définit une valeur indiquant si la hauteur de la ligne d'en-tête du tableau peut être ajustée. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Obtient ou définit le format de date du tableau. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Obtient ou définit une valeur indiquant si la première colonne d'un tableau est verrouillée ou modifiable. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Obtient ou définit le nom d'un objet Table. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Obtient ou définit la hauteur des lignes dans un tableau, où la hauteur des lignes correspond au nombre de lignes de texte. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher l'interface 'Add New Column'. Pris en charge à partir de la version MSP 2010 et suivantes. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Obtient ou définit une valeur indiquant si le projet affiche le nom du tableau dans la liste déroulante Tables de l'onglet Affichage du ruban. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Obtient une collection TableFields représentant les champs du tableau. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Obtient ou définit le type de tableau pour le tableau spécifié. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Obtient l'identifiant unique d'une table. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Renvoie un code de hachage pour cette Table. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


