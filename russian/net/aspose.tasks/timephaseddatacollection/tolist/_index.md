---
title: "TimephasedDataCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TimephasedDataCollection. Преобразует объект TimephasedDataCollection в список объектов TimephasedData"
type: docs
weight: 120
url: /ru/net/aspose.tasks/timephaseddatacollection/tolist/
---
## TimephasedDataCollection.ToList method

Преобразует объект [`TimephasedDataCollection`](../) в список объектов [`TimephasedData`](../../timephaseddata/).

```csharp
public List<TimephasedData> ToList()
```

### Возвращаемое значение

Список объектов [`TimephasedData`](../../timephaseddata/).

## Примеры

Показывает, как работать с коллекциями данных по фазам времени.

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

// установить контурную форму работы
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

Console.WriteLine("Is timephased data collection read-only?: " + assignment.TimephasedData.IsReadOnly);

// очистить сгенерированные tds
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

// можно отфильтровать коллекцию по типу и диапазону дат
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
// добавьте неверный td, а затем удалите его
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

// удалите неверный элемент td
if (assignment.TimephasedData.Contains(td4))
{
    assignment.TimephasedData.Remove(td4);
}

// ...
assignment.TimephasedData.AddRange(list);

// итерация по элементам timephased
Console.WriteLine("Print all timephased items:");
Console.WriteLine("Timephased data count: " + assignment.TimephasedData.Count);
foreach (var item in assignment.TimephasedData)
{
    Console.WriteLine("Start: " + item.Start);
    Console.WriteLine("Finish: " + item.Finish);
    Console.WriteLine("Timephased Data Type: " + item.TimephasedDataType);
    Console.WriteLine();
}

// скопируйте tds в другое назначение
var timephasedDatas = new TimephasedData[assignment.TimephasedData.Count];
assignment.TimephasedData.CopyTo(timephasedDatas, 0);

assignment2.TimephasedData.Clear();
foreach (var data in timephasedDatas)
{
    assignment2.TimephasedData.Add(data);
}

// коллекцию можно преобразовать в простой список
List<TimephasedData> tds = assignment.TimephasedData.ToList();

// удалим tds по одному
foreach (var timephasedData in tds)
{
    assignment.TimephasedData.Remove(timephasedData);
}
```

### См. также

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* namespace [Aspose.Tasks](../../timephaseddatacollection/)
* assembly [Aspose.Tasks](../../../)


