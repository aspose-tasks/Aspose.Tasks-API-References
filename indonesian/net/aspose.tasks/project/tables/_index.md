---
title: "Project.Tables"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan daftar objek Table"
type: docs
weight: 900
url: /id/net/aspose.tasks/project/tables/
---
## Project.Tables property

Mendapatkan daftar objek [`Table`](../../table/).

```csharp
public TableCollection Tables { get; }
```

## Contoh

Menampilkan cara mengkonfigurasi properti Gantt Chart.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // Define new custom attribute
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // Add custom text attribute to created task.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // Sesuaikan tabel dengan menambahkan bidang atribut teks
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

### Lihat Juga

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


