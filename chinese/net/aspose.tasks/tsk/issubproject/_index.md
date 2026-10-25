---
title: "Tsk.IsSubproject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否为插入的子项目"
type: docs
weight: 700
url: /zh/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

确定任务是否为插入的项目。

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## 示例

展示如何读取/写入 Tsk.IsSubproject 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


