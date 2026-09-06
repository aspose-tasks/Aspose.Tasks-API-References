---
title: "Duration.ToString"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 方法。返回此实例的字符串表示形式。"
type: docs
weight: 120
url: /zh/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

返回此实例的字符串表示。

```csharp
public override string ToString()
```

### 返回值

此实例的字符串表示形式。

## 示例

展示如何将 Duration 转换为字符串。

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// 获取任务的 Duration。
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


