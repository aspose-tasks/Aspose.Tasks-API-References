---
title: "Table.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Table. تُرجع رمز تجزئة لهذا Table"
type: docs
weight: 130
url: /ar/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

يعيد رمز تجزئة لهذا الجدول.

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

يعيد قيمة رمز التجزئة لهذا الكائن.

## الأمثلة

يظهر كيفية الحصول على رمز تجزئة لجدول.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// رمز التجزئة لجدول يساوي معرف UID للجدول 
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### انظر أيضًا

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


