---
title: "Project.Tables"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-eigenschap. Haalt een lijst met Table-objecten op"
type: docs
weight: 900
url: /nl/net/aspose.tasks/project/tables/
---
## Project.Tables property

Haalt een lijst met [`Table`](../../table/) objecten op.

```csharp
public TableCollection Tables { get; }
```

## Voorbeelden

Toont hoe Gantt Chart-eigenschappen te configureren.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // Definieer een nieuw aangepast attribuut
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // Voeg een aangepast tekstattribuut toe aan de aangemaakte taak.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // Pas de tabel aan door een tekstattribuutveld toe te voegen
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

### Zie ook

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


