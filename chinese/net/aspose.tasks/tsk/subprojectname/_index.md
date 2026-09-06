---
title: "Tsk.SubprojectName"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。子项目的源位置"
type: docs
weight: 1070
url: /zh/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

子项目的源位置。

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## 示例

展示如何创建子项目任务。

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// 添加任务
var task = project.RootTask.Children.Add("Task 1");

// 设置新的子项目链接
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


