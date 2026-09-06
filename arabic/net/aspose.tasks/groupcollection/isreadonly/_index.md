---
title: "GroupCollection.IsReadOnly"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GroupCollection. تُرجع قيمة تُشير إلى ما إذا كان هذا التجميع للقراءة فقط"
type: docs
weight: 20
url: /ar/net/aspose.tasks/groupcollection/isreadonly/
---
## GroupCollection.IsReadOnly property

يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط.

```csharp
public bool IsReadOnly { get; }
```

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

* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


