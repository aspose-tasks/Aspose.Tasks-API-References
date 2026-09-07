---
title: "Project.Tables"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει μια λίστα αντικειμένων Table"
type: docs
weight: 900
url: /el/net/aspose.tasks/project/tables/
---
## Project.Tables property

Λαμβάνει μια λίστα αντικειμένων [`Table`](../../table/).

```csharp
public TableCollection Tables { get; }
```

## Παραδείγματα

Δείχνει πώς να διαμορφώσετε τις ιδιότητες του Gantt Chart.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // Ορίστε νέο προσαρμοσμένο χαρακτηριστικό
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // Προσθέστε προσαρμοσμένο χαρακτηριστικό κειμένου στην δημιουργημένη εργασία.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // Προσαρμόστε τον πίνακα προσθέτοντας πεδίο χαρακτηριστικού κειμένου
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

### Δείτε επίσης

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


