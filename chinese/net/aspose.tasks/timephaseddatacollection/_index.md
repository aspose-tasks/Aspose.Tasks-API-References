---
title: "类 TimephasedDataCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TimephasedDataCollection 类。表示一个 TimephasedData 对象的集合"
type: docs
weight: 2600
url: /zh/net/aspose.tasks/timephaseddatacollection/
---
## TimephasedDataCollection class

表示一个 [`TimephasedData`](../timephaseddata/) 对象的集合。

```csharp
public abstract class TimephasedDataCollection : IList<TimephasedData>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/timephaseddatacollection/count/) { get; } | 获取此 `TimephasedDataCollection` 对象中包含的对象数量。 |
| [IsReadOnly](../../aspose.tasks/timephaseddatacollection/isreadonly/) { get; } | 获取一个值，指示 ICollection 是否为只读。 |
| [Item](../../aspose.tasks/timephaseddatacollection/item/) { get; set; } | 返回指定索引处的元素。不支持 set 访问器。属性用于设置分阶段数据。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/timephaseddatacollection/add/)(TimephasedData) | 向此集合对象添加 [`TimephasedData`](../timephaseddata/) 实例。 |
| [AddRange](../../aspose.tasks/timephaseddatacollection/addrange/)(IEnumerable&lt;TimephasedData&gt;) | 向此集合对象添加一组 [`TimephasedData`](../timephaseddata/) 实例。 |
| [Clear](../../aspose.tasks/timephaseddatacollection/clear/)() | 从 `TimephasedDataCollection` 中移除所有项。 |
| [Contains](../../aspose.tasks/timephaseddatacollection/contains/)(TimephasedData) | 确定 `TimePhasedDataCollection` 是否包含特定值。 |
| [CopyTo](../../aspose.tasks/timephaseddatacollection/copyto/)(TimephasedData[], int) | 将 `TimephasedDataCollection` 的元素复制到数组中，从特定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/timephaseddatacollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/timephaseddatacollection/remove/)(TimephasedData) | 从此集合对象中移除 [`TimephasedData`](../timephaseddata/) 实例。 |
| [SelectBetweenStartAndFinish](../../aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/)(TimephasedDataType, DateTime, DateTime) | 选择 *startTime* 与 *finishTime* 之间的所有时间阶段。平均情况下具有 O(log n) 的复杂度。 |
| [ToList](../../aspose.tasks/timephaseddatacollection/tolist/)() | 将 `TimephasedDataCollection` 对象转换为 [`TimephasedData`](../timephaseddata/) 对象的列表。 |

## 示例

展示如何使用分阶段数据集合。

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

// 设置等高工作轮廓
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

Console.WriteLine("Is timephased data collection read-only?: " + assignment.TimephasedData.IsReadOnly);

// 清除生成的 tds
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

// 可以按类型和日期范围过滤集合
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
// 添加一个错误的 td 然后删除它
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

// 删除错误的 td 项目
if (assignment.TimephasedData.Contains(td4))
{
    assignment.TimephasedData.Remove(td4);
}

// ...
assignment.TimephasedData.AddRange(list);

// 遍历时间分段项目
Console.WriteLine("Print all timephased items:");
Console.WriteLine("Timephased data count: " + assignment.TimephasedData.Count);
foreach (var item in assignment.TimephasedData)
{
    Console.WriteLine("Start: " + item.Start);
    Console.WriteLine("Finish: " + item.Finish);
    Console.WriteLine("Timephased Data Type: " + item.TimephasedDataType);
    Console.WriteLine();
}

// 将 td 复制到另一个分配
var timephasedDatas = new TimephasedData[assignment.TimephasedData.Count];
assignment.TimephasedData.CopyTo(timephasedDatas, 0);

assignment2.TimephasedData.Clear();
foreach (var data in timephasedDatas)
{
    assignment2.TimephasedData.Add(data);
}

// 该集合可以转换为普通列表
List<TimephasedData> tds = assignment.TimephasedData.ToList();

// 让我们逐个删除 td
foreach (var timephasedData in tds)
{
    assignment.TimephasedData.Remove(timephasedData);
}
```

### 另见

* class [TimephasedData](../timephaseddata/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


