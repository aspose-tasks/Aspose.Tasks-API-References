---
title: "枚举 TaskType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskType 枚举。指定任务的类型。"
type: docs
weight: 2470
url: /zh/net/aspose.tasks/tasktype/
---
## TaskType enumeration

指定任务的类型。

```csharp
public enum TaskType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 未定义的值表示该字段在原始文件中未定义 |
| FixedUnits | `0` | 固定单位 |
| FixedDuration | `1` | 固定持续时间 |
| FixedWork | `2` | 固定工作量 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

展示如何读取项目的默认属性。

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// 设置默认属性
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// 显示默认属性
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


