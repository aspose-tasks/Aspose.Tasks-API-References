---
title: "TableField.AlignTitle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TableField. تحصل أو تعين محاذاة العنوان في حقل جدول"
type: docs
weight: 30
url: /ar/net/aspose.tasks/tablefield/aligntitle/
---
## TableField.AlignTitle property

يحصل أو يعيّن محاذاة العنوان في حقل جدول.

```csharp
public HorizontalStringAlignment AlignTitle { get; set; }
```

## الأمثلة

يوضح كيفية قراءة جداول المشروع.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// احصل على الجدول
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// عرض جميع معلومات حقول الجدول
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### انظر أيضًا

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


