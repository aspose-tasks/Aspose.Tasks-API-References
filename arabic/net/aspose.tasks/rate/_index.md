---
title: "الفئة Rate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Rate. تمثل تعريفًا لفترة زمنية والأسعار المطبقة على مورد خلال تلك الفترة"
type: docs
weight: 1610
url: /ar/net/aspose.tasks/rate/
---
## Rate class

يمثل تعريف فترة زمنية والأسعار المطبقة على مورد خلال تلك الفترة.

```csharp
public class Rate
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | يحصل أو يعيّن تكلفة الاستخدام للمورد. يتم استرجاع هذه القيمة من التاريخ الحالي إذا كان هناك جدول أسعار للمورد. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | يحصل أو يعيّن معدل العمل الإضافي للساعة للمورد. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | يحصل أو يعيّن الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | يحصل أو يعيّن التاريخ الذي يصبح فيه السعر ساريًا. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | يحصل أو يعيّن آخر تاريخ يكون فيه السعر ساريًا. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | يحصل أو يعيّن المعرف الفريد لجدول الأسعار للمورد. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | يحصل أو يعيّن السعر القياسي للساعة للمورد. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | يحصل أو يعيّن الوحدات التي يستخدمها Microsoft Project لعرض السعر القياسي. |

## الأمثلة

يعرض كيفية التعامل مع أسعار الموارد.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// العمل مع المشروع...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


