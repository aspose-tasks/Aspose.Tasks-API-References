---
title: "Duration.Parse"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تقوم بتحويل السلسلة المحددة إلى نسخة من بنية Duration."
type: docs
weight: 10
url: /ar/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

يقوم بتحويل السلسلة المحددة إلى نسخة من بنية [`Duration`](../).

```csharp
public static Duration Parse(Project p, string value)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| p | Project | النسخة المحددة من الفئة [`Project`](../../project/) لتحويل المدة لها. |
| value | سلسلة | السلسلة المحددة للتحويل. |

### قيمة الإرجاع

يعيد النسخة المحوّلة من بنية [`Duration`](../).

## الأمثلة

يظهر كيفية تحليل نص من نص مُنسق بشكل خاص.

```csharp
var project = new Project();

// أمثلة على المدد:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// حيث 1 - عدد العناصر (يوم، أسبوع، إلخ)، d - يوم (h - ساعة، w - أسبوع) ? - علامة تقديرية، e - علامة منقضية

// حاول تحليل مدة تقديرية
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// حاول تحليل مدة تقديرية
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### انظر أيضًا

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


