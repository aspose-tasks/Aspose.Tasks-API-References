---
title: "ResourceCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "ResourceCollection method. تحول كائن ResourceCollection إلى قائمة من كائنات Resource"
type: docs
weight: 100
url: /ar/net/aspose.tasks/resourcecollection/tolist/
---
## ResourceCollection.ToList method

تحول كائن ResourceCollection إلى قائمة من كائنات [`Resource`](../../resource/).

```csharp
public List<Resource> ToList()
```

### قيمة الإرجاع

قائمة من كائنات [`Resource`](../../resource/).

## الأمثلة

يوضح كيفية العمل مع مجموعات الموارد.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// إضافة مورد فارغ
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// إضافة مورد باسم
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// إضافة مورد قبل المورد بالمعرف المحدد
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// الحصول على مورد بالمعرف
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// مجموعات الموارد لا تدعم عملية Clear
// project.Resources.Clear();
// استخدم عينة الكود التالية بدلاً من ذلك
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### انظر أيضًا

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


