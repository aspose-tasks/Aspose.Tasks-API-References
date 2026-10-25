---
title: "TreeAlgorithmBase1.PostAlg"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TreeAlgorithmBase. تُستدعى بعد معالجة عقدة في شجرة."
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/treealgorithmbase-1/postalg/
---
## TreeAlgorithmBase&lt;T&gt;.PostAlg method

يُستدعى بعد معالجة عقدة في شجرة.

```csharp
public virtual void PostAlg(T el, int level)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| el | T | العقدة للمعالجة. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


