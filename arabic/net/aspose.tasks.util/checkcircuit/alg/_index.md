---
title: "CheckCircuit.Alg"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CheckCircuit. تحقق مما إذا كان الكائن المحدد قد تم معالجته مسبقاً"
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

تحقق مما إذا كان الكائن المحدد قد تم معالجته بالفعل.

```csharp
public override void Alg(Task el, int level)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| el | مهمة | الكائن للمعالجة. |
| المستوى | Int32 | مستوى عقدة الشجرة. |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


