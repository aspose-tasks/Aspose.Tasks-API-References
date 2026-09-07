---
title: "Duration.TimeUnit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration प्रॉपर्टी। इस ऑब्जेक्ट के लिए समय इकाई प्रकार प्राप्त करता है। इस Duration इंस्टेंस की समय इकाई प्रकार।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

इस ऑब्जेक्ट के लिए समय इकाई प्रकार प्राप्त करता है। इस Duration इंस्टेंस का समय इकाई प्रकार।

```csharp
public TimeUnitType TimeUnit { get; }
```

## उदाहरण

कार्य की अवधि को कैसे अपडेट करें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// एक कार्य प्राप्त करें
var task1 = project.RootTask.Children.GetById(1);

// कार्य की अवधि अपडेट करें
var duration1 = task1.Get(Tsk.Duration);

// कार्य 1 में एक दिन जोड़ें
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// कार्य के लिए नई अवधि सेट करें
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// एक और कार्य प्राप्त करें
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// वास्तविक समय इकाई प्रकार का उपयोग करके अवधि बदलें
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// कार्य के लिए नई अवधि सेट करें
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### संबंधित देखें

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


