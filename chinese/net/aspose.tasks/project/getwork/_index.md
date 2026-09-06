---
title: "Project.GetWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。获取具有指定 Double 值和默认工作格式的 Duration 对象"
type: docs
weight: 1130
url: /zh/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

获取 [`Duration`](../../duration/) 对象，使用指定的 Double 值和默认工作格式。

```csharp
public Duration GetWork(double val)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | Double | 指定的 double 值。 |

### 返回值

Duration 对象。

## 备注

此方法应谨慎使用，因为它根据 Project.WorkFormat 设置返回不同的持续时间。例如，当 Project.WorkFormat 为 TimeUnitType.Hour 时，GetWork(1.0) 将返回 1 小时；如果 Project.WorkFormat 为 TimeUnitType.Day，则返回 1 天。

## 示例

展示如何使用默认工作格式获取工作。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// 使用项目的默认工作格式创建工作值
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### 另见

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


