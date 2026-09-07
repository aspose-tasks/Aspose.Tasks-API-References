---
title: "Duration.TimeSpan"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration प्रॉपर्टी। इस Duration ऑब्जेक्ट का TimeSpan इंस्टेंस प्राप्त करता है। इस Duration ऑब्जेक्ट का TimeSpan इंस्टेंस।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

`TimeSpan` इंस्टेंस इस Duration ऑब्जेक्ट का प्राप्त करता है। इस Duration ऑब्जेक्ट का TimeSpan इंस्टेंस।

```csharp
public TimeSpan TimeSpan { get; }
```

## उदाहरण

अवधि को टाइम स्पैन में बदलने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// कार्य की अवधि प्राप्त करें
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### संबंधित देखें

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


