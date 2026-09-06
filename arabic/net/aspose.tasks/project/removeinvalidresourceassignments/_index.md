---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تُزيل التعيينات غير الصالحة للموارد من قائمة تعيينات موارد المشروع"
type: docs
weight: 1170
url: /ar/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

يقوم بإزالة تعيينات الموارد غير الصالحة من قائمة تعيينات موارد المشروع.

```csharp
public void RemoveInvalidResourceAssignments()
```

## ملاحظات

يقوم MS Project بإنشاء تعيين مورد فارغ لكل مهمة. استدعِ الطريقة لإزالتها.

## الأمثلة

يعرض كيفية إزالة التعيينات غير الصالحة.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// إزالة التعيينات غير الصالحة
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


