---
title: "Resource.ParentProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Resource. يحصل على المشروع الأب لهذه الحاوية"
type: docs
weight: 600
url: /ar/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

يحصل على المشروع الأب لهذه الحاوية.

```csharp
public Project ParentProject { get; }
```

## الأمثلة

يعرض كيفية استخدام المشروع الأب للموارد.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// تعيين عمل للمورد باستخدام نوع وحدة زمنية للعمل في المشروع الافتراضي.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### انظر أيضًا

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


