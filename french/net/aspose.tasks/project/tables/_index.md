---
title: "Project.Tables"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Project. Obtient une liste d'objets Table"
type: docs
weight: 900
url: /fr/net/aspose.tasks/project/tables/
---
## Project.Tables property

Obtient une liste d'objets [`Table`](../../table/).

```csharp
public TableCollection Tables { get; }
```

## Exemples

Montre comment configurer les propriétés du Gantt Chart.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // Définir un nouvel attribut personnalisé
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // Ajouter un attribut texte personnalisé à la tâche créée.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // Personnalisez la table en ajoutant un champ d'attribut texte
    var field = new TableField
    {
        Field = Field.TaskText1,
        Width = 20,
        Title = "Custom attribute",
        AlignTitle = HorizontalStringAlignment.Center,
        AlignData = HorizontalStringAlignment.Center
    };

    var table = project.Tables.ToList()[0];
    table.TableFields.Insert(3, field);

    project.Save(OutDir + @"ConfigureGantChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
}
catch (NotSupportedException ex)
{
    Console.WriteLine(
        ex.Message
        + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http:// Www.aspose.com/purchase/default.aspx.");
}
```

### Voir aussi

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


