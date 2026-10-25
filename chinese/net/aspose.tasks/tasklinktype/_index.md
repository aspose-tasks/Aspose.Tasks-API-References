---
title: "枚举 TaskLinkType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskLinkType 枚举。指定任务依赖的类型。"
type: docs
weight: 2440
url: /zh/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

指定任务依赖的类型。

```csharp
public enum TaskLinkType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| FinishToFinish | `0` | 结束-结束关系 |
| FinishToStart | `1` | 结束-开始关系 |
| StartToFinish | `2` | 开始-结束关系 |
| StartToStart | `3` | 开始-开始关系 |

## 示例

展示如何获取/设置任务链接的链接类型。

```csharp
var project = new Project();

// 添加新任务
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// 将任务链接设置为开始-开始类型进行链接
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


