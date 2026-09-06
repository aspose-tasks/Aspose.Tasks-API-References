---
title: "Resource.TimephasedData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Resource. تحصل أو تعين مثيل من الفئة TimephasedDataCollection لهذا الكائن."
type: docs
weight: 740
url: /ar/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

يحصل أو يعيّن نسخة من الفئة [`TimephasedDataCollection`](../../timephaseddatacollection/) لهذا الكائن.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## ملاحظات

القراءة مدعومة لتنسيق XML فقط.

## الأمثلة

يوضح كيفية قراءة بيانات الوقت المرحلية للمورد.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// التكرار عبر بيانات الوقت المرحلية للمورد
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


