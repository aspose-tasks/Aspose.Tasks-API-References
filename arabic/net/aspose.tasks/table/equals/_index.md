---
title: "Table.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Table. تُرجع قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد"
type: docs
weight: 120
url: /ar/net/aspose.tasks/table/equals/
---
## Table.Equals method

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## الأمثلة

يظهر كيفية التحقق من مساواة الجدول.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// يتم التحقق من مساواة الجداول مقابل معرف UID الخاص بالجدول.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### انظر أيضًا

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


