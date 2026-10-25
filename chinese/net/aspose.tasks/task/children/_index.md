---
title: "Task.Children"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取此对象的子任务集合。TaskCollection 对象，表示子任务。"
type: docs
weight: 190
url: /zh/net/aspose.tasks/task/children/
---
## Task.Children property

获取此对象的子任务集合。TaskCollection 对象，表示子任务。

```csharp
public TaskCollection Children { get; }
```

## 示例

展示如何使用任务集合添加任务。

```csharp
var project = new Project();

// 添加任务、子任务并保存项目
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### 另见

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


