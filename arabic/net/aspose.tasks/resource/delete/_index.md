---
title: "Resource.Delete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Resource. تحذف موردًا وتعييناته من المشروع"
type: docs
weight: 810
url: /ar/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

يحذف موردًا وتعييناته من المشروع.

```csharp
public void Delete()
```

## الأمثلة

يوضح كيفية حذف مورد.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// احذف المورد
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### انظر أيضًا

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


