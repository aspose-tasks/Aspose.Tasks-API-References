---
title: "ResourceAssignment.MakeTPs"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। समय-फ़ेज़्ड डेटा की सूची उत्पन्न करता है"
type: docs
weight: 740
url: /hi/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

टाइम‑फ़ेज़्ड डेटा की सूची उत्पन्न करता है।

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | निर्दिष्ट प्रारंभ तिथि। |
| समय | TimeSpan | निर्दिष्ट कार्य समय। |
| कैलेंडर | कैलेंडर | निर्दिष्ट कार्य कैलेंडर। |
| सूची | List`1 | समय-फ़ेज़्ड डेटा की सूची। |
| isWorking | Boolean | निर्दिष्ट फ़्लैग जो निर्धारित करता है कि समय-फ़ेज़्ड डेटा कार्यरत है या नहीं। |
| प्रकार | Int32 | निर्दिष्ट समय-फ़ेज़्ड डेटा प्रकार। |

### रिटर्न वैल्यू

सूची से अधिकतम तिथि या यदि सूची खाली है तो प्रारंभ तिथि।

## उदाहरण

पैरामीटर द्वारा TPs उत्पन्न करने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### संबंधित देखें

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


