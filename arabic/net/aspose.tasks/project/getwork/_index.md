---
title: "Project.GetWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تحصل على كائن Duration بالقيمة Double المحددة وتنسيق العمل الافتراضي"
type: docs
weight: 1130
url: /ar/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

تحصل على كائن [`Duration`](../../duration/) بالقيمة Double المحددة وتنسيق العمل الافتراضي.

```csharp
public Duration GetWork(double val)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| القيمة | Double | القيمة double المحددة. |

### قيمة الإرجاع

كائن Duration.

## ملاحظات

يجب استخدام هذه الطريقة بحذر لأنها تُعيد فترات زمنية مختلفة اعتمادًا على إعداد Project.WorkFormat. على سبيل المثال، GetWork(1.0) سيعيد 1 ساعة عندما يكون Project.WorkFormat هو TimeUnitType.Hour أو 1 يوم إذا كان Project.WorkFormat هو TimeUnitType.Day.

## الأمثلة

يظهر كيفية الحصول على عمل بتنسيق العمل الافتراضي.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// إنشاء قيمة عمل باستخدام تنسيق العمل الافتراضي للمشروع
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### انظر أيضًا

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


