---
title: "ResourceAssignment.Guid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ResourceAssignment. تحصل أو تعين المعرف الفريد لهذا التعيين"
type: docs
weight: 290
url: /ar/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

يحصل أو يعيّن المعرف الفريد لهذا التكليف.

```csharp
public Guid? Guid { get; set; }
```

## الأمثلة

يوضح كيفية قراءة GUID لتعيين المورد.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### انظر أيضًا

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


