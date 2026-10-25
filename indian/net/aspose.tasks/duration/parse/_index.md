---
title: "Duration.Parse"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration मेथड। निर्दिष्ट स्ट्रिंग को Duration स्ट्रक्ट के इंस्टेंस में परिवर्तित करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

निर्दिष्ट स्ट्रिंग को [`Duration`](../) स्ट्रक्ट के इंस्टेंस में परिवर्तित करता है।

```csharp
public static Duration Parse(Project p, string value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| p | Project | निर्दिष्ट [`Project`](../../project/) क्लास के इंस्टेंस को अवधि बदलने के लिए। |
| value | स्ट्रिंग | परिवर्तित करने के लिए निर्दिष्ट स्ट्रिंग। |

### रिटर्न वैल्यू

परिवर्तित [`Duration`](../) स्ट्रक्ट का इंस्टेंस लौटाता है।

## उदाहरण

विशेष रूप से स्वरूपित स्ट्रिंग से स्ट्रिंग को पार्स करने का तरीका दर्शाता है।

```csharp
var project = new Project();

// duration के उदाहरण:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// जहाँ 1 - आइटमों की संख्या (दिन, सप्ताह, आदि), d - दिन (h - घंटा, w - सप्ताह) ? - अनुमानित फ़्लैग, e - समाप्त फ़्लैग

// एक अनुमानित duration को पार्स करने का प्रयास करें
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// एक अनुमानित duration को पार्स करने का प्रयास करें
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### संबंधित देखें

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


