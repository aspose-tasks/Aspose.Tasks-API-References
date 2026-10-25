---
title: "Duration.IsEstimated"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration प्रॉपर्टी। यह एक मान प्राप्त करता है जो दर्शाता है कि समय इकाई अनुमानित है या नहीं। वह फ़्लैग जो निर्धारित करता है कि यह Duration instance अनुमानित है या नहीं।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/duration/isestimated/
---
## Duration.IsEstimated property

एक मान प्राप्त करता है जो दर्शाता है कि समय इकाई अनुमानित है या नहीं। वह फ़्लैग जो निर्धारित करता है कि यह Duration उदाहरण अनुमानित है या नहीं।

```csharp
public bool IsEstimated { get; }
```

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


