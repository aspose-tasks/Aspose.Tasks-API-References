---
title: "Duration.Add"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration मेथड। इस अवधि में निर्दिष्ट अवधि जोड़ता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks/duration/add/
---
## Add(Duration) {#add}

निर्दिष्ट अवधि को इस अवधि में जोड़ता है।

```csharp
public Duration Add(Duration d)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| d | Duration | इस इंस्टेंस में जोड़ने के लिए निर्दिष्ट [`Duration`](../)। |

### रिटर्न वैल्यू

यह नया duration ऑब्जेक्ट इस उदाहरण के मान को निर्दिष्ट duration मान के साथ जोड़कर दर्शाता है।

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Add(double) {#add_1}

निर्दिष्ट डबल मान को इस अवधि में जोड़ता है।

```csharp
public Duration Add(double val)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | Double | निर्दिष्ट Double मान जिसे इस उदाहरण में जोड़ना है। |

### रिटर्न वैल्यू

यह नया duration ऑब्जेक्ट इस उदाहरण के मान को निर्दिष्ट duration मान के साथ जोड़कर दर्शाता है।

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


