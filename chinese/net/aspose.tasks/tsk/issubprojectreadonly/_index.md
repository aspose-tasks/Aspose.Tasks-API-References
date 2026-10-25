---
title: "Tsk.IsSubprojectReadOnly"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定子项目是否为只读"
type: docs
weight: 710
url: /zh/net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

确定子项目是否为只读。

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## 示例

展示如何读取/写入 Tsk.IsSubprojectReadOnly 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


