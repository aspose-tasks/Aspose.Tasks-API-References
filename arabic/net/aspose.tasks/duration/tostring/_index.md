---
title: "Duration.ToString"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تُرجع تمثيلًا نصيًا لهذه المثيلة."
type: docs
weight: 120
url: /ar/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

يعيد تمثيلًا نصيًا لهذا الكائن.

```csharp
public override string ToString()
```

### قيمة الإرجاع

تمثيل نصي لهذه المثيلة.

## الأمثلة

يظهر كيفية تحويل مدة إلى نص.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// احصل على مدة المهمة
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### انظر أيضًا

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


