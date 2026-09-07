---
title: "क्लास TimephasedDataCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TimephasedDataCollection class. TimephasedData ऑब्जेक्ट्स का संग्रह दर्शाता है"
type: docs
weight: 2600
url: /hi/net/aspose.tasks/timephaseddatacollection/
---
## TimephasedDataCollection class

एक संग्रह दर्शाता है [`TimephasedData`](../timephaseddata/) ऑब्जेक्ट्स।

```csharp
public abstract class TimephasedDataCollection : IList<TimephasedData>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/timephaseddatacollection/count/) { get; } | इस `TimephasedDataCollection` ऑब्जेक्ट में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/timephaseddatacollection/isreadonly/) { get; } | ICollection पढ़ने‑के‑लिए‑केवल है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [Item](../../aspose.tasks/timephaseddatacollection/item/) { get; set; } | निर्दिष्ट अनुक्रमांक पर तत्व लौटाता है। सेट एक्सेसर समर्थित नहीं है। timephased डेटा सेट करने की प्रॉपर्टी। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/timephaseddatacollection/add/)(TimephasedData) | जोड़ता है [`TimephasedData`](../timephaseddata/) उदाहरण इस संग्रह ऑब्जेक्ट में। |
| [AddRange](../../aspose.tasks/timephaseddatacollection/addrange/)(IEnumerable&lt;TimephasedData&gt;) | इस संग्रह ऑब्जेक्ट में [`TimephasedData`](../timephaseddata/) उदाहरणों का संग्रह जोड़ता है। |
| [Clear](../../aspose.tasks/timephaseddatacollection/clear/)() | `TimephasedDataCollection` से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/timephaseddatacollection/contains/)(TimephasedData) | निर्धारित करता है कि `TimephasedDataCollection` में कोई विशिष्ट मान है या नहीं। |
| [CopyTo](../../aspose.tasks/timephaseddatacollection/copyto/)(TimephasedData[], int) | `TimephasedDataCollection` के तत्वों को एक Array में कॉपी करता है, एक विशिष्ट Array अनुक्रमांक से शुरू करके। |
| [GetEnumerator](../../aspose.tasks/timephaseddatacollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/timephaseddatacollection/remove/)(TimephasedData) | इस संग्रह ऑब्जेक्ट से [`TimephasedData`](../timephaseddata/) उदाहरण हटाता है। |
| [SelectBetweenStartAndFinish](../../aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/)(TimephasedDataType, DateTime, DateTime) | सभी time phases को *startTime* और *finishTime* के बीच चुनता है। औसत केस में O(log n) जटिलता है। |
| [ToList](../../aspose.tasks/timephaseddatacollection/tolist/)() | `TimephasedDataCollection` ऑब्जेक्ट को [`TimephasedData`](../timephaseddata/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

timephased डेटा संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var resource2 = project.Resources.Add("Resource 2");
resource2.Set(Rsc.Type, ResourceType.Work);

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2019, 11, 11, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.Work, project.GetDuration(3d, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2019, 11, 11, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Work, project.GetDuration(3d, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2019, 11, 11, 8, 0, 0));
assignment.Set(Asn.Work, project.GetDuration(3, TimeUnitType.Hour));
assignment.Set(Asn.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var assignment2 = project.ResourceAssignments.Add(task2, resource2);
assignment2.Set(Asn.Start, new DateTime(2019, 11, 11, 8, 0, 0));
assignment2.Set(Asn.Work, project.GetDuration(3, TimeUnitType.Hour));
assignment2.Set(Asn.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

// सेट कंटूरयुक्त कार्य कंटूर
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

Console.WriteLine("Is timephased data collection read-only?: " + assignment.TimephasedData.IsReadOnly);

// जेनरेटेड tds साफ़ करें
assignment.TimephasedData.Clear();

var td = new TimephasedData
             {
                 Start = new DateTime(2019, 11, 11, 8, 0, 0),
                 Finish = new DateTime(2019, 11, 11, 9, 0, 0),
                 Uid = assignment.Get(Asn.Uid),
                 Unit = TimeUnitType.Hour,
                 Value = "PT1H0M0S",
                 TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
             };
assignment.TimephasedData.Add(td);

var list = new List<TimephasedData>();
var td2 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 12, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 12, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT1H0M0S",
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };
var td3 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 13, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 13, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT1H0M0S",
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };

list.Add(td2);
list.Add(td3);
assignment.TimephasedData.AddRange(list);

// संग्रह को प्रकार और तिथि सीमा द्वारा फ़िल्टर किया जा सकता है।
Console.WriteLine("Print filtered tds:");
IList<TimephasedData> filteredTds = assignment.TimephasedData.SelectBetweenStartAndFinish(
    TimephasedDataType.AssignmentRemainingWork,
    new DateTime(2019, 11, 11, 0, 0, 0),
    new DateTime(2019, 11, 13));
foreach (var data in filteredTds)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("Timephased Data Type: " + data.TimephasedDataType);
    Console.WriteLine();
}

Console.WriteLine("--------------------------");
Console.WriteLine();

// ...
// एक गलत td जोड़ें और फिर उसे हटाएँ
var td4 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 13, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 13, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT0H0M1S", // wrong value
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };
assignment.TimephasedData.Add(td4);

// ...

// गलत td आइटम को हटाएँ
if (assignment.TimephasedData.Contains(td4))
{
    assignment.TimephasedData.Remove(td4);
}

// ...
assignment.TimephasedData.AddRange(list);

// timephased आइटम्स पर इटररेट करें
Console.WriteLine("Print all timephased items:");
Console.WriteLine("Timephased data count: " + assignment.TimephasedData.Count);
foreach (var item in assignment.TimephasedData)
{
    Console.WriteLine("Start: " + item.Start);
    Console.WriteLine("Finish: " + item.Finish);
    Console.WriteLine("Timephased Data Type: " + item.TimephasedDataType);
    Console.WriteLine();
}

// tds को दूसरे असाइनमेंट में कॉपी करें
var timephasedDatas = new TimephasedData[assignment.TimephasedData.Count];
assignment.TimephasedData.CopyTo(timephasedDatas, 0);

assignment2.TimephasedData.Clear();
foreach (var data in timephasedDatas)
{
    assignment2.TimephasedData.Add(data);
}

// कलेक्शन को साधारण सूची में बदला जा सकता है
List<TimephasedData> tds = assignment.TimephasedData.ToList();

// आइए tds को एक-एक करके हटाएँ
foreach (var timephasedData in tds)
{
    assignment.TimephasedData.Remove(timephasedData);
}
```

### संबंधित देखें

* class [TimephasedData](../timephaseddata/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


