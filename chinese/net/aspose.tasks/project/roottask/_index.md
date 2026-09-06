---
title: "Project.RootTask"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取任务树的根节点"
type: docs
weight: 800
url: /zh/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

获取任务树的根节点。

```csharp
public Task RootTask { get; }
```

## 示例

展示如何通过使用根项目任务向项目中添加任务。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### 另见

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


