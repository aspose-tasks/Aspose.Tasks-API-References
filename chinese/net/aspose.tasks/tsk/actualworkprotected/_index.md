---
title: "Tsk.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。实际工作受保护的持续时间。仅支持 XML 格式的读取"
type: docs
weight: 100
url: /zh/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

实际工作受到保护的持续时间。仅支持 XML 格式的读取。

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## 示例

展示如何读取/写入 Tsk.ActualWorkProtected 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


