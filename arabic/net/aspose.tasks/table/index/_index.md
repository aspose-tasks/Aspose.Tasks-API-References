---
title: "Table.Index"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Table. تحصل على فهرس كائن Table في كائن Tables الحاوي"
type: docs
weight: 40
url: /ar/net/aspose.tasks/table/index/
---
## Table.Index property

يحصل على فهرس كائن Table في كائن Tables الحاوي.

```csharp
public int Index { get; }
```

## الأمثلة

يعرض كيفية تعريف جدول جديد (يُستخدم للعرض).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// احصل على جدول للتعديل
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Index of the table: " + table.Index);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// ضبط بعض الخصائص
// تعيين قيمة تشير إلى ما إذا كان يمكن تعديل ارتفاع صف الرأس في الجدول
table.AdjustHeaderRowHeight = true;

// تعيين تنسيق التاريخ للجدول.
table.DateFormat = DateFormat.DateDdMmYyyy;

// تعيين قيمة تشير إلى ما إذا كان العمود الأول في الجدول مقفلاً أو قابلًا للتعديل
table.LockFirstColumn = true;

// تعيين ارتفاع الصف في جدول، حيث يكون ارتفاع الصف هو عدد أسطر النص
table.RowHeight = 10;

// يحدد قيمة تشير إلى ما إذا كان يجب عرض واجهة 'Add New Column'
table.ShowAddNewColumn = true;

// تعيين قيمة تشير إلى ما إذا كان المشروع يعرض اسم الجدول في القائمة المنسدلة للجداول على علامة تبويب العرض في الشريط
table.ShowInMenu = true;

// يسمح بحفظ الجدول المحدث
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


