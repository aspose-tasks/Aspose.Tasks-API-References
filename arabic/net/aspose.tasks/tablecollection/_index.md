---
title: "الفئة TableCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TableCollection. تحتوي على قائمة من كائنات Table. تنفّذ واجهة ICollectionTable."
type: docs
weight: 2330
url: /ar/net/aspose.tasks/tablecollection/
---
## TableCollection class

تحتوي على قائمة من كائنات [`Table`](../table/) . تنفّذ واجهة ICollection&lt;Table&gt;.

```csharp
public class TableCollection : ICollection<Table>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | يحوّل مجموعة الجداول إلى قائمة من كائنات [`Table`](../table/). |

## الأمثلة

يظهر كيفية العمل مع مجموعات الجداول.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// التنقل عبر الجداول
Console.WriteLine("Print tables of " + project.Get(Prj.Name) + " project.");
Console.WriteLine("Table count: " + project.Tables.Count);
foreach (var tbl in project.Tables)
{
    Console.WriteLine("Name: " + tbl.Name);

    Console.WriteLine("Fields:");

    foreach (var field in tbl.TableFields)
    {
        Console.WriteLine("    {0} - '{1}' - {2}", field.Field, field.Title, field.Width);
    }
}

// إضافة جدول جديد
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// يمكن مسح المجموعة بطريقتين
if (deleteOneByOne)
{
    // نسخ الجداول إلى المصفوفة وحذفها واحدةً تلو الأخرى
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // أو يمكن مسح مجموعة الجداول بالكامل
    project.Tables.Clear();
}

// يمكن تحويل المجموعة إلى قائمة بسيطة من الجداول
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### انظر أيضًا

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


