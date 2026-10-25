---
title: "स्ट्रक्ट Duration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Duration स्ट्रक्ट। एक प्रोजेक्ट में अवधि का प्रतिनिधित्व करता है।"
type: docs
weight: 470
url: /hi/net/aspose.tasks/duration/
---
## Duration structure

परियोजना में अवधि का प्रतिनिधित्व करता है।

```csharp
public struct Duration : IEquatable<Duration>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि समय इकाई समाप्त हुई है या नहीं। वह फ़्लैग जो निर्धारित करता है कि यह Duration उदाहरण समाप्त हुआ है या नहीं। |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि समय इकाई अनुमानित है या नहीं। वह फ़्लैग जो निर्धारित करता है कि यह Duration उदाहरण अनुमानित है या नहीं। |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | इस Duration ऑब्जेक्ट की [`TimeSpan`](./timespan/) इंस्टेंस प्राप्त करता है। इस Duration ऑब्जेक्ट की TimeSpan इंस्टेंस। |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | इस ऑब्जेक्ट के लिए समय इकाई प्रकार प्राप्त करता है। इस Duration इंस्टेंस का समय इकाई प्रकार। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | निर्दिष्ट स्ट्रिंग को `Duration` स्ट्रक्ट की इंस्टेंस में परिवर्तित करता है। |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | निर्दिष्ट डबल मान को इस अवधि में जोड़ता है। |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | निर्दिष्ट अवधि को इस अवधि में जोड़ता है। |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Duration ऑब्जेक्ट को निर्दिष्ट समय इकाइयों के साथ दूसरी अवधि में परिवर्तित करता है। |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है। |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | निर्दिष्ट डबल मान को इस अवधि इंस्टेंस से घटाता है। |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | निर्दिष्ट अवधि को इस अवधि इंस्टेंस से घटाता है। |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Duration ऑब्जेक्ट को Double मान में परिवर्तित करता है। |
| override [ToString](../../aspose.tasks/duration/tostring/)() | इस इंस्टेंस का स्ट्रिंग प्रतिनिधित्व लौटाता है। |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | "PT--H--M--S--" प्रारूप में अवधि स्ट्रिंग को पार्स करता है। |
| [operator ==](../../aspose.tasks/duration/op_equality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


