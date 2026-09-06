---
title: "Task.TimephasedData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. الحصول أو تعيين كائن TimephasedDataCollection لهذه المهمة. كتلة البيانات الزمنية المرتبطة بالمهمة"
type: docs
weight: 1220
url: /ar/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

يحصل أو يعيّن كائن TimephasedDataCollection لهذه المهمة. كتلة البيانات الزمنية المرتبطة بالمهمة.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## ملاحظات

القراءة مدعومة لتنسيق XML فقط.

## الأمثلة

يوضح كيفية التكرار عبر البيانات الزمنية للمهمة.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


