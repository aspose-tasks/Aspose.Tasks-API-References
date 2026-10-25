---
title: "Duration.ParseTimeSpan"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تقوم بتحليل سلسلة المدة بالتنسيق PTHMS."
type: docs
weight: 130
url: /ar/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

يحلل سلسلة المدة بالتنسيق "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| value | سلسلة | السلسلة المحددة للتحليل. |

### قيمة الإرجاع

يعيد نسخة مُحلَّلة من بنية [`TimeSpan`](../timespan/).

## الأمثلة

يظهر كيفية تحويل سلسلة نصية إلى فترة زمنية.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### انظر أيضًا

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


