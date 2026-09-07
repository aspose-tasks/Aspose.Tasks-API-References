---
title: "Project.Tables"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Restituisce un elenco di oggetti Table"
type: docs
weight: 900
url: /it/net/aspose.tasks/project/tables/
---
## Project.Tables property

Restituisce un elenco di oggetti [`Table`](../../table/).

```csharp
public TableCollection Tables { get; }
```

## Esempi

Mostra come configurare le proprietà del Gantt Chart.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // Definisci un nuovo attributo personalizzato
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // Aggiungi un attributo di testo personalizzato al task creato.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // Personalizza la tabella aggiungendo il campo attributo di testo
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

### Vedi anche

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


