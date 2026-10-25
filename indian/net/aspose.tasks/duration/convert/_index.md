---
title: "Duration.Convert"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration मेथड। निर्दिष्ट समय इकाइयों के साथ Duration ऑब्जेक्ट को दूसरी अवधि में बदलता है।"
type: docs
weight: 70
url: /hi/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Duration ऑब्जेक्ट को निर्दिष्ट समय इकाइयों के साथ दूसरी अवधि में परिवर्तित करता है।

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| timeUnitType | TimeUnitType | निर्दिष्ट समय इकाई प्रकार। |

### रिटर्न वैल्यू

निर्दिष्ट इकाई प्रकार के साथ नया duration लौटाता है।

## उदाहरण

दिखाता है कि अवधि को विभिन्न समय इकाई प्रकारों में कैसे बदलें।

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// एक कार्य प्राप्त करें ताकि उसकी अवधि को विभिन्न स्वरूपों में गणना किया जा सके
var task = project.RootTask.Children.GetById(1);

// मिनट, दिन, घंटे, सप्ताह और महीने में अवधि प्राप्त करें
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### संबंधित देखें

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


