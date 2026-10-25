---
title: "Project.Tables"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على قائمة من كائنات Table"
type: docs
weight: 900
url: /ar/net/aspose.tasks/project/tables/
---
## Project.Tables property

تحصل على قائمة من كائنات [`Table`](../../table/)

```csharp
public TableCollection Tables { get; }
```

## الأمثلة

يعرض كيفية تكوين خصائص مخطط Gantt.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // تعريف سمة مخصصة جديدة.
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // أضف سمة نص مخصصة إلى المهمة التي تم إنشاؤها.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // تخصيص الجدول عن طريق إضافة حقل سمة النص
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

### انظر أيضًا

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


