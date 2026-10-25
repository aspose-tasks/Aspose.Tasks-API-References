---
title: "Task.RecurringInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task property. कार्य के लिए RecurringTaskInfo क्लास का इंस्टेंस प्राप्त करता है, जो कि एक आवर्ती कार्य है; यदि कार्य आवर्ती नहीं है तो null लौटाता है। RecurringTaskInfo के इंस्टेंस की जानकारी केवल mpp फ़ाइल फ़ॉर्मेट में उपलब्ध है।"
type: docs
weight: 1030
url: /hi/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

कार्य के लिए [`RecurringTaskInfo`](../../recurringtaskinfo/) क्लास का इंस्टेंस प्राप्त करता है, जो एक आवर्ती कार्य है; यदि कार्य आवर्ती नहीं है तो null लौटाता है; [`RecurringTaskInfo`](../../recurringtaskinfo/) के इंस्टेंस की जानकारी केवल mpp फ़ाइल फ़ॉर्मेट में उपलब्ध है।

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## उदाहरण

दिखाता है कि कार्य की आवर्ती जानकारी कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Recurrence Pattern: " + task.RecurringInfo.RecurrencePattern);
Console.WriteLine("Start Date: " + task.RecurringInfo.StartDate);
Console.WriteLine("End Date: " + task.RecurringInfo.EndDate);
Console.WriteLine("Duration: " + task.RecurringInfo.Duration);
Console.WriteLine("Occurrences: " + task.RecurringInfo.Occurrences);
Console.WriteLine("Weekly Days: " + task.RecurringInfo.WeeklyDays);
Console.WriteLine("WeeklyRepetitions: " + task.RecurringInfo.WeeklyRepetitions);
```

### संबंधित देखें

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


