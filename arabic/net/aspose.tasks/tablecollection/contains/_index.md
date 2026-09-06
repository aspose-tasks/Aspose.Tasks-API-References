---
title: "TableCollection.Contains"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TableCollection. تُرجِع true إذا تم العثور على العنصر المحدد في هذه المجموعة وإلا false"
type: docs
weight: 50
url: /ar/net/aspose.tasks/tablecollection/contains/
---
## TableCollection.Contains method

يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false.

```csharp
public bool Contains(Table item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | Table | العنصر المحدد للبحث عنه. |

### قيمة الإرجاع

صحيح إذا وُجد العنصر المحدد في هذه المجموعة؛ وإلا، خطأ.

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

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


