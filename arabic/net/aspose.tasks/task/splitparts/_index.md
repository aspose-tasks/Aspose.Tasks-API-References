---
title: "Task.SplitParts"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. تحصل على مجموعة SplitPart التي تمثل أجزاء المهمة"
type: docs
weight: 1110
url: /ar/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

يحصل على مجموعة SplitPart التي تمثل أجزاء المهمة.

```csharp
public SplitPartCollection SplitParts { get; }
```

## الأمثلة

يظهر كيفية عرض أجزاء المهمة المقسمة.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// الوصول إلى المهمة 
var task = project.RootTask.Children.GetById(4);

// عرض أجزاء المهمة المقسمة
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### انظر أيضًا

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


