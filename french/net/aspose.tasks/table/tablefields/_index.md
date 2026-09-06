---
title: "Table.TableFields"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Table. Obtient une collection TableFields représentant les champs de la table"
type: docs
weight: 90
url: /fr/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Obtient une collection TableFields représentant les champs du tableau.

```csharp
public TableFieldCollection TableFields { get; }
```

## Exemples

Montre comment travailler avec les tables du projet.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Définir un nouvel attribut personnalisé
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Ajouter un attribut texte personnalisé à la tâche créée.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Personnalisez la table en ajoutant un champ d'attribut texte
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Voir aussi

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


