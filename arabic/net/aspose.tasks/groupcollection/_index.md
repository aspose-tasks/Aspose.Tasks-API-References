---
title: "الفئة GroupCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.GroupCollection. تحتوي على قائمة من كائنات Group. تنفذ واجهة ICollectionGroup."
type: docs
weight: 780
url: /ar/net/aspose.tasks/groupcollection/
---
## GroupCollection class

تحتوي على قائمة من كائنات [`Group`](../group/) . تنفذ واجهة ICollection&lt;Group&gt;.

```csharp
public class GroupCollection : ICollection<Group>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | يحوّل مجموعة المجموعات إلى قائمة من كائنات [`Group`](../group/) . |

## الأمثلة

يوضح كيفية العمل مع مجموعة من المجموعات.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// التكرار عبر مجموعات المهام
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// التكرار عبر مجموعات الموارد
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// مسح مجموعات المشروع الآخر
otherProject.TaskGroups.Clear();

// نسخ المجموعات إلى مشروع آخر
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// إضافة مجموعة مهام مخصصة
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// إزالة جميع المجموعات
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### انظر أيضًا

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


