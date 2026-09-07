---
title: "Calendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। कार्य की समाप्ति तिथि और समय की गणना उसके प्रारंभ तिथि के विभाजित भागों और कार्य अवधि से करता है"
type: docs
weight: 210
url: /hi/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

कार्य की प्रारंभ तिथि, विभाजित भागों और कार्य अवधि से समाप्ति तिथि और समय की गणना करता है।

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | कार्य | जिस कार्य की समाप्ति तिथि की गणना करनी है। |
| अवधि | TimeSpan | जिस अवधि की गणना करनी है। |

### रिटर्न वैल्यू

दिए गए प्रारंभ तिथि और अवधि के लिए कार्य की समाप्ति तिथि।

## टिप्पणियाँ

यदि कार्य सारांश है, null है या उसकी प्रारंभ तिथि सेट नहीं है तो DateTime.MinValue लौटाता है।

## उदाहरण

कस्टम अवधि द्वारा कार्य की समाप्ति तिथि की गणना कैसे करें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "SplitTaskFinishDate.mpp");

// एक विभाजित कार्य खोजें
var task = project.RootTask.Children.GetByUid(4);

// प्रोजेक्ट कैलेंडर खोजें
var calendar = project.Get(Prj.Calendar);

// विभिन्न अवधियों के साथ कार्य की समाप्ति तिथि की गणना करें
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 8 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(8, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 16 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(16, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 24 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(24, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 28 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(28, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 32 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(32, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 46 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(46, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 61 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(61, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 75 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(75, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 80 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(80, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 120 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(120, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 150 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(150, 0, 0)));
```

### संबंधित देखें

* class [Task](../../task/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


