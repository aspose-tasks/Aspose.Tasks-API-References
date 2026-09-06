---
title: "TableFieldCollection.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TableFieldCollection. تُضيف العنصر المحدد إلى هذه المجموعة."
type: docs
weight: 40
url: /ar/net/aspose.tasks/tablefieldcollection/add/
---
## TableFieldCollection.Add method

يضيف العنصر المحدد إلى هذه المجموعة.

```csharp
public void Add(TableField item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | TableField | العنصر المحدد لإضافته إلى هذه المجموعة. |

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

* class [TableField](../../tablefield/)
* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


