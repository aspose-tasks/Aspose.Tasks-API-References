---
title: "Filter.CompareTo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Filter. تقارن هذه النسخة بالنسخة المحددة من فئة Filter وتعيد إشارة إلى ترتيبها النسبي"
type: docs
weight: 90
url: /ar/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

تقارن هذه النسخة بالنسخة المحددة من فئة [`Filter`](../) وتعيد إشارة إلى ترتيبها النسبي.

```csharp
public int CompareTo(Filter other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| other | Filter | النسخة المحددة من فئة [`Filter`](../) للمقارنة مع هذا الكائن. |

### قيمة الإرجاع

إشارة إلى ترتيبها النسبي.

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


