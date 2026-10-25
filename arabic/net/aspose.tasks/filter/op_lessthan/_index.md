---
title: "Filter.op_LessThan"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Filter. تُرجع قيمة تشير إلى ما إذا كانت هذه المثيلة أصغر من كائن محدد"
type: docs
weight: 160
url: /ar/net/aspose.tasks/filter/op_lessthan/
---
## Filter LessThan operator

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من كائن محدد.

```csharp
public static bool operator <(Filter a, Filter b)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| a | Filter | المرشح الأول. |
| b | Filter | المرشح الثاني. |

### قيمة الإرجاع

قيمة تشير إلى ما إذا كانت هذه المثيلة أصغر من كائن محدد

## الأمثلة

يظهر كيفية فحص مساواة المرشح.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// يتم فحص مساواة المرشحات مقابل معرف الـ UID للمرشح.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### انظر أيضًا

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


