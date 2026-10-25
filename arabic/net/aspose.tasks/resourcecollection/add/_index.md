---
title: "ResourceCollection.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceCollection. تُضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع"
type: docs
weight: 40
url: /ar/net/aspose.tasks/resourcecollection/add/
---
## Add() {#add}

يضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع.

```csharp
public Resource Add()
```

### قيمة الإرجاع

تمت إضافة المورد.

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

---

## Add(string) {#add_1}

يضيف موردًا جديدًا في الموضع الأخير من مجموعة موارد المشروع.

```csharp
public Resource Add(string resourceName)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| resourceName | سلسلة | اسم المورد. |

### قيمة الإرجاع

تمت إضافة المورد.

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

---

## Add(string, int) {#add_2}

يضيف موردًا جديدًا في الموضع المحدد من مجموعة موارد المشروع.

```csharp
public Resource Add(string resourceName, int beforeResourceId)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| resourceName | سلسلة | اسم المورد. |
| beforeResourceId | Int32 | موضع المورد السابق في مجموعة موارد المشروع. |

### قيمة الإرجاع

تمت إضافة المورد.

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


