---
title: "الفئة TableFieldCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TableFieldCollection. تحتوي على قائمة من كائنات TableField. تنفّذ واجهة IListTableField."
type: docs
weight: 2350
url: /ar/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

تحتوي على قائمة من كائنات [`TableField`](../tablefield/) . تنفّذ واجهة IList&lt;TableField&gt;.

```csharp
public class TableFieldCollection : IList<TableField>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | يرجع أو يعيّن العنصر في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | يحدد فهرس العنصر المحدد في هذه المجموعة. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | يدرج العنصر المحدد في الفهرس المحدد. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | يزيل عنصرًا في الفهرس المحدد. |

## الأمثلة

يوضح كيفية العمل مع مجموعات حقول الجدول.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // التكرار عبر حقول الجدول
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// إضافة حقل جدول جديد
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// إدراج حقل جديد في الموضع
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// دعنا نحرّر حقل الجدول الجديد باستخدام الوصول عبر الفهرس
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// مؤخرًا يمكننا إزالة الحقل
table.TableFields.RemoveAt(idx);

// يمكن مسح المجموعة بطريقتين
if (deleteOneByOne)
{
    // نسخ حقول الجدول إلى المصفوفة وحذفها واحدةً تلو الأخرى
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // أو يمكن للمرء مسح مجموعة حقول الجدول بالكامل
    table.TableFields.Clear();
}
```

### انظر أيضًا

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


