---
title: "CheckCircuit.CheckCircuit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ CheckCircuit. يهيئ مثيلاً جديداً من الفئة CheckCircuit"
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

يهيئ مثيلاً جديداً من الفئة [`CheckCircuit`](../).

```csharp
public CheckCircuit()
```

## الأمثلة

يوضح كيفية اكتشاف بنية المشروع المكسورة.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// تحقق من بنية المشروع.
// سيتم رمي <see cref=\"TasksException\"> إذا كانت بنية المشروع غير صحيحة.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### انظر أيضًا

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


