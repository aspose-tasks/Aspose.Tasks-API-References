---
title: "Tsk.CommitmentType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否具有关联的交付或对关联交付的依赖。仅支持 XML 格式的读取。"
type: docs
weight: 190
url: /zh/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

确定任务是否具有关联的交付或对关联交付的依赖。仅支持 XML 格式的读取。

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## 示例

展示如何读取/写入 Tsk.CommitmentType 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


