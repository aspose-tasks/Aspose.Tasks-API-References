---
title: "Duration.Subtract"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration मेथड। निर्दिष्ट अवधि को इस अवधि इंस्टेंस से घटाता है।"
type: docs
weight: 100
url: /hi/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

निर्दिष्ट अवधि को इस अवधि इंस्टेंस से घटाता है।

```csharp
public Duration Subtract(Duration d)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| d | Duration | इस इंस्टेंस से घटाने के लिए निर्दिष्ट [`Duration`](../) इंस्टेंस। |

### रिटर्न वैल्यू

नया अवधि ऑब्जेक्ट जो इस इंस्टेंस के मान को निर्दिष्ट अवधि मान घटाकर दर्शाता है।

## उदाहरण

कार्य की अवधि को बदलने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// एक कार्य प्राप्त करें
var task1 = project.RootTask.Children.GetById(1);

// कार्य की अवधि अपडेट करें
var duration1 = task1.Get(Tsk.Duration);

// कार्य 1 के लिए एक दिन घटाएँ।
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// कार्य के लिए नई अवधि सेट करें
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// एक और कार्य प्राप्त करें
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// वास्तविक समय इकाई प्रकार का उपयोग करके अवधि बदलें
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// कार्य के लिए नई अवधि सेट करें
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### संबंधित देखें

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

निर्दिष्ट डबल मान को इस अवधि इंस्टेंस से घटाता है।

```csharp
public Duration Subtract(double val)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | Double | इस इंस्टेंस से घटाने के लिए निर्दिष्ट Double मान। |

### रिटर्न वैल्यू

नया अवधि ऑब्जेक्ट जो इस इंस्टेंस के मान को निर्दिष्ट अवधि मान घटाकर दर्शाता है।

## उदाहरण

कार्य की अवधि को बदलने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// एक कार्य प्राप्त करें
var task1 = project.RootTask.Children.GetById(1);

// कार्य की अवधि अपडेट करें
var duration1 = task1.Get(Tsk.Duration);

// कार्य 1 के लिए एक दिन घटाएँ।
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// कार्य के लिए नई अवधि सेट करें
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// एक और कार्य प्राप्त करें
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// वास्तविक समय इकाई प्रकार का उपयोग करके अवधि बदलें
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// कार्य के लिए नई अवधि सेट करें
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### संबंधित देखें

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


