---
title: "Tsk.CommitmentType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المهمة لديها تسليم مرتبط أو اعتماد على تسليم مرتبط. القراءة مدعومة فقط لتنسيق XML"
type: docs
weight: 190
url: /ar/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

يحدد ما إذا كانت المهمة لديها تسليم مرتبط أو اعتماد على تسليم مرتبط. القراءة مدعومة فقط لتنسيق XML.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.CommitmentType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


