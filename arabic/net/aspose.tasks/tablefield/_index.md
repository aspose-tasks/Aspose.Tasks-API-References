---
title: "الفئة TableField"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.TableField. تمثل حقلًا في جدول داخل مشروع."
type: docs
weight: 2340
url: /ar/net/aspose.tasks/tablefield/
---
## TableField class

يمثّل حقلًا في جدول داخل مشروع.

```csharp
public class TableField
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TableField](tablefield/)() | ينشئ مثلاً جديداً من الفئة `TableField`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | يحصل أو يعيّن محاذاة البيانات في حقل جدول. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | يحصل أو يعيّن محاذاة العنوان في حقل جدول. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | يحصل أو يعيّن نوع حقل جدول. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | يحصل أو يعيّن عنوان الحقل في جدول. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | يحصل أو يعيّن عرض العمود بالوحدات النقطية للحقل في جدول. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان عنوان عمود الجدول يمكن أن يلتف إلى عدة أسطر، أو إذا يجب قصه عندما يتجاوز عرض العمود. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نص العمود يمكن أن يلتف إلى عدة أسطر، أو إذا يجب قطعه عندما يتجاوز عرض العمود. مدعوم في نسخة MSP 2010 وما بعدها. |

## الأمثلة

يوضح كيفية العمل مع عرض Project وإضافة عمود إلى العرض الافتراضي (الذي يُظهر عندما يُفتح ملف MPP في MS Project).

```csharp
// إنشاء مشروع فارغ بدون عروض
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// تعديل العرض الافتراضي (إنه عرض مخطط جانت).
// أو يمكنك اختيار العرض بالاسم أو عبر شاشة العرض باستخدام مجموعة project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// يجب استخدام علم WriteViewData لحفظ تعديلات خصائص العرض.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


