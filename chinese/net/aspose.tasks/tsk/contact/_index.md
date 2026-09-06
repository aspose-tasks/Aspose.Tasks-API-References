---
title: "Tsk.Contact"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。负责任务的个人姓名"
type: docs
weight: 220
url: /zh/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

任务负责人的姓名。

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## 示例

展示如何读取/写入 Tsk.Contact 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


