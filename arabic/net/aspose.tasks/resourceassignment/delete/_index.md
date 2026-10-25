---
title: "ResourceAssignment.Delete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تحذف تعيين المورد من مجموعة تعيينات المشروع"
type: docs
weight: 680
url: /ar/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

يحذف تعيين المورد من مجموعة تعيينات المشروع.

```csharp
public void Delete()
```

## الأمثلة

يعرض كيفية حذف تعيين مورد.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### انظر أيضًا

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


