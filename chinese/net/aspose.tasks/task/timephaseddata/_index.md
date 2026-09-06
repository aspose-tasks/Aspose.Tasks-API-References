---
title: "Task.TimephasedData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取或设置此任务的 TimephasedDataCollection 对象。与任务关联的时间分段数据块"
type: docs
weight: 1220
url: /zh/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

获取或设置此任务的 TimephasedDataCollection 对象。与任务关联的时间分段数据块。

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## 备注

仅支持 XML 格式的读取。

## 示例

展示如何遍历任务的时间分段数据。

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


