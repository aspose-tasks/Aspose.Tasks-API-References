---
title: "ResourceAssignment.ParentProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ResourceAssignment. تحصل على المشروع الأب لهذا التعيين"
type: docs
weight: 420
url: /ar/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

يحصل على المشروع الأصل لهذا التكليف.

```csharp
public Project ParentProject { get; }
```

## الأمثلة

يظهر كيفية استخدام المشروع الأب لتعيين مورد.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// تعيين مدة التعيين باستخدام نوع وحدة الوقت الافتراضية للمشروع.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### انظر أيضًا

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


