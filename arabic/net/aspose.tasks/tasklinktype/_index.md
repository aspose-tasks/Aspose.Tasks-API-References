---
title: "التعداد TaskLinkType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.TaskLinkType. يحدد نوع تبعية المهام"
type: docs
weight: 2440
url: /ar/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

يحدد نوع تبعية المهام.

```csharp
public enum TaskLinkType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| FinishToFinish | `0` | علاقة الانتهاء-الانتهاء |
| FinishToStart | `1` | علاقة الانتهاء-البداية |
| StartToFinish | `2` | علاقة البداية-الانتهاء |
| StartToStart | `3` | علاقة البداية-البداية |

## الأمثلة

يعرض كيفية الحصول على/تعيين نوع ارتباط مهمة.

```csharp
var project = new Project();

// إضافة مهام جديدة
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// ربط المهام بنوع ارتباط محدد إلى البداية إلى البداية
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


