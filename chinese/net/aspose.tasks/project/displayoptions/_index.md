---
title: "Project.DisplayOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取 ProjectDisplayOptions 类的实例"
type: docs
weight: 380
url: /zh/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

获取 [`ProjectDisplayOptions`](../../projectdisplayoptions/) 类的实例。

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## 示例

展示如何调优项目的显示选项。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 设置一个值，指示当 Project 检测到手动安排的任务可能出现调度冲突时是否显示警告。
// 此选项适用于 Project 2010 及更高版本。
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### 另见

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


