---
title: "TaskLink.LinkType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskLink. تحصل أو تعين نوع الرابط"
type: docs
weight: 60
url: /ar/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

يحصل أو يعيّن نوع الرابط.

```csharp
public TaskLinkType LinkType { get; set; }
```

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

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


