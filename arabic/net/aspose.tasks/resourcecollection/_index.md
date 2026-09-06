---
title: "الفئة ResourceCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ResourceCollection. تمثل مجموعة من كائنات Resource."
type: docs
weight: 1770
url: /ar/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

يمثل مجموعة من كائنات [`Resource`](../resource/).

```csharp
public class ResourceCollection : IList<Resource>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | يحصل على عدد العناصر الموجودة في ResourceCollection. Int32 للقراءة فقط. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | يحصل على المشروع الأب لكائن ResourceCollection. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | يضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | يضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | يضيف موردًا جديدًا في الموضع المحدد من مجموعة موارد المشروع. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | المسح المباشر غير مدعوم، هذه الطريقة فقط تُطلق NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | يرجع موردًا بالمعرف المحدد. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | يرجع موردًا بالمعرف الفريد المحدد. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | هذه هي تنفيذية النموذجية لطريقة Remove في ICollection، التي ترمي فقط NotSupportedException |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | يحول كائن ResourceCollection إلى قائمة من كائنات [`Resource`](../resource/). |

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

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


