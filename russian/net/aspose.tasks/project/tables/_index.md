---
title: "Project.Tables"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Возвращает список объектов Table"
type: docs
weight: 900
url: /ru/net/aspose.tasks/project/tables/
---
## Project.Tables property

Возвращает список объектов [`Table`](../../table/).

```csharp
public TableCollection Tables { get; }
```

## Примеры

Показывает, как настроить свойства Gantt Chart.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // Определить новый пользовательский атрибут
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // Добавить пользовательский текстовый атрибут к созданной задаче.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // Настройте таблицу, добавив поле текстового атрибута
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

### См. также

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


