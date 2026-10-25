---
title: "الفئة CheckCircuit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Util.CheckCircuit. تتحقق من شجرة المهام ما إذا كانت تحتوي على دائرة."
type: docs
weight: 2680
url: /ar/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

يفحص شجرة (من المهام) لمعرفة ما إذا كانت تحتوي على دائرة.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | يُنشئ مثيلًا جديدًا للفئة `CheckCircuit`. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | تحقق مما إذا كان الكائن المحدد قد تم معالجته بالفعل. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


