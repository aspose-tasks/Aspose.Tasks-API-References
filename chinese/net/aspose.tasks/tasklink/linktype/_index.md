---
title: "TaskLink.LinkType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLink 属性。获取或设置链接的类型"
type: docs
weight: 60
url: /zh/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

获取或设置链接的类型。

```csharp
public TaskLinkType LinkType { get; set; }
```

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

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


