---
title: "एनम BookingType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.BookingType एनम। संसाधन के बुकिंग प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 150
url: /hi/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

संसाधन के बुकिंग प्रकार को निर्दिष्ट करता है।

```csharp
public enum BookingType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | मूल प्रोजेक्ट फ़ाइल में मान परिभाषित नहीं था, यह दर्शाता है। |
| Committed | `0` | Committed बुकिंग प्रकार को दर्शाता है। |
| Proposed | `1` | Proposed बुकिंग प्रकार को दर्शाता है। |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि Asn.BookingType प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


