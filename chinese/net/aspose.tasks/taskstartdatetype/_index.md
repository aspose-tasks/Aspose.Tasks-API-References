---
title: "枚举 TaskStartDateType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskStartDateType 枚举。指定任务开始日期的类型"
type: docs
weight: 2450
url: /zh/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

指定任务开始日期的类型。

```csharp
public enum TaskStartDateType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 字段的值未在原始项目文件中定义。 |
| ProjectStartDate | `0` | 项目开始日期 |
| CurrentDate | `1` | 当前日期 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

展示如何将任务的默认开始日期设置为 'CurrentDate'。

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


