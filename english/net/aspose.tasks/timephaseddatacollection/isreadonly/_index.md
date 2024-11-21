---
title: TimephasedDataCollection.IsReadOnly
second_title: Aspose.Tasks for .NET API Reference
description: TimephasedDataCollection property. Gets a value indicating whether the ICollection is readonly
type: docs
weight: 20
url: /net/aspose.tasks/timephaseddatacollection/isreadonly/
---
## TimephasedDataCollection.IsReadOnly property

Gets a value indicating whether the ICollection is read-only.

```csharp
public bool IsReadOnly { get; }
```

### Return Value

true if the ICollection is read-only; otherwise, false.

## Examples

Shows how to work with timephased data collections.

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

// set contoured work contour
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

Console.WriteLine("Is timephased data collection read-only?: " + assignment.TimephasedData.IsReadOnly);

// clear generated tds
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

// one can filter the collection by type and date range
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
// add a wrong td and then delete it
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

// delete the wrong td item
if (assignment.TimephasedData.Contains(td4))
{
    assignment.TimephasedData.Remove(td4);
}

// ...
assignment.TimephasedData.AddRange(list);

// iterate over timephased items
Console.WriteLine("Print all timephased items:");
Console.WriteLine("Timephased data count: " + assignment.TimephasedData.Count);
foreach (var item in assignment.TimephasedData)
{
    Console.WriteLine("Start: " + item.Start);
    Console.WriteLine("Finish: " + item.Finish);
    Console.WriteLine("Timephased Data Type: " + item.TimephasedDataType);
    Console.WriteLine();
}

// copy tds to another assignment
var timephasedDatas = new TimephasedData[assignment.TimephasedData.Count];
assignment.TimephasedData.CopyTo(timephasedDatas, 0);

assignment2.TimephasedData.Clear();
foreach (var data in timephasedDatas)
{
    assignment2.TimephasedData.Add(data);
}

// the collection can be converted to a plain list
List<TimephasedData> tds = assignment.TimephasedData.ToList();

// lets remove tds one by one
foreach (var timephasedData in tds)
{
    assignment.TimephasedData.Remove(timephasedData);
}
```

### See Also

* class [TimephasedDataCollection](../)
* namespace [Aspose.Tasks](../../timephaseddatacollection/)
* assembly [Aspose.Tasks](../../../)


