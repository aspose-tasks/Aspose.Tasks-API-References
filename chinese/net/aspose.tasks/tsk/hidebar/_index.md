---
title: "Tsk.HideBar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定在 Microsoft Project 中显示时任务的甘特条是否隐藏"
type: docs
weight: 480
url: /zh/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

确定在 Microsoft Project 中显示时，任务的甘特条是否被隐藏。

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## 示例

展示如何读取/写入 Tsk.HideBar 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


