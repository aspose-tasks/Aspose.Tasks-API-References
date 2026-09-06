---
title: "Filter.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Filter. تُرجع قيمة تشير إلى ما إذا كانت هذه النسخة مساوية لكائن AssignmentBaseline المحدد."
type: docs
weight: 100
url: /ar/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية للكيان AssignmentBaseline المحدد.

```csharp
public bool Equals(Filter other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | Filter | كائن AssignmentBaseline المحدد للمقارنة مع هذه النسخة. |

### قيمة الإرجاع

تُرجع true إذا كانت هذه النسخة مساوية لكائن AssignmentBaseline المحدد؛ وإلا، false.

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

---

## Equals(object) {#equals_1}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية للكيان AssignmentBaseline المحدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | كائن AssignmentBaseline المحدد للمقارنة مع هذه النسخة. |

### قيمة الإرجاع

تُرجع true إذا كانت هذه النسخة مساوية لكائن AssignmentBaseline المحدد؛ وإلا، false.

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


