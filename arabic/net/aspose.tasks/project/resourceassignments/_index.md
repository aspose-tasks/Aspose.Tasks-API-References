---
title: "Project.ResourceAssignments"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على كائن ResourceAssignmentCollection"
type: docs
weight: 750
url: /ar/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

يحصل على كائن ResourceAssignmentCollection.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## الأمثلة

يوضح كيفية العمل مع تعيينات الموارد.

```csharp
var project = new Project();

// إضافة مهمة وموارد جديدة
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// تعيين المورد للمهمة المطلوبة
project.ResourceAssignments.Add(task, resource);
```

### انظر أيضًا

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


