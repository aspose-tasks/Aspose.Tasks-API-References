---
title: "Duration.IsElapsed"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Duration. تحصل على قيمة تشير إلى ما إذا كانت وحدة الوقت منقضية. العلامة التي تحدد ما إذا كانت هذه المثيلة من Duration منقضية."
type: docs
weight: 20
url: /ar/net/aspose.tasks/duration/iselapsed/
---
## Duration.IsElapsed property

يحصل على قيمة تشير إلى ما إذا كانت وحدة الوقت منقضية. العلامة التي تحدد ما إذا كان هذا المثيل من Duration منقضيًا.

```csharp
public bool IsElapsed { get; }
```

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


