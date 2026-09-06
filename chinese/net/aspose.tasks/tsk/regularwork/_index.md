---
title: "Tsk.RegularWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。资源计划执行的非加班工作总量"
type: docs
weight: 940
url: /zh/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

资源计划执行的非加班工作总量。

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## 示例

展示如何读取/写入 Tsk.RegularWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


