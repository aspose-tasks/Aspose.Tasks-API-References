---
title: "Project.Tables"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Table nesnelerinin bir listesini alır."
type: docs
weight: 900
url: /tr/net/aspose.tasks/project/tables/
---
## Project.Tables property

[`Table`](../../table/) nesnelerinin bir listesini alır.

```csharp
public TableCollection Tables { get; }
```

## Örnekler

Gantt Chart özelliklerini nasıl yapılandıracağını gösterir.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // Yeni özel öznitelik tanımla
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // Oluşturulan göreve özel metin özniteliği ekle.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // Tabloyu metin özelliği alanı ekleyerek özelleştirin
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

### Ayrıca Bakınız

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


