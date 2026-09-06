---
title: "الفئة Table"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Table. تمثل جدولاً في Project."
type: docs
weight: 2320
url: /ar/net/aspose.tasks/table/
---
## Table class

يمثل جدولًا في Project

```csharp
public class Table
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Table](table/)() | يُنشئ مثلاً جديداً من الفئة `Table`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يمكن تعديل ارتفاع صف الرأس في الجدول. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | يحصل أو يعيّن تنسيق التاريخ للجدول. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان العمود الأول في الجدول مقفلاً أو قابلاً للتحرير. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | يحصل أو يعيّن اسم كائن Table. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | يحصل أو يعيّن ارتفاع الصف في جدول، حيث يكون ارتفاع الصف هو عدد أسطر النص. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إظهار واجهة 'Add New Column'. مدعومة في نسخة MSP 2010 وما بعدها. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان المشروع يعرض اسم الجدول في القائمة المنسدلة Tables في تبويب View على الشريط. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | يحصل على مجموعة TableFields التي تمثل الحقول في الجدول. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | يحصل أو يعيّن نوع الجدول للجدول المحدد. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | يحصل على المعرف الفريد للجدول. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | يعيد رمز تجزئة لهذا الجدول. |

## الأمثلة

يعرض كيفية تعريف جدول جديد (يُستخدم للعرض).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// احصل على جدول للتعديل
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


