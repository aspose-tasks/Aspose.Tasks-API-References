---
title: "Group.ShowInMenu"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Group. تحصل أو تعين قيمة تشير إلى ما إذا كان Project يعرض اسم المجموعة في القائمة المنسدلة Group في الشريط"
type: docs
weight: 60
url: /ar/net/aspose.tasks/group/showinmenu/
---
## Group.ShowInMenu property

يحصل أو يضبط قيمة تشير إلى ما إذا كان Project يعرض اسم المجموعة في القائمة المنسدلة Group في الشريط.

```csharp
public bool ShowInMenu { get; set; }
```

## الأمثلة

يعرض كيفية العمل مع المجموعات.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Uid: " + group.Uid);
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Is Task Group Maintain Hierarchy?: " + group.MaintainHierarchy);
Console.WriteLine("Is Task Group Show In Menu?: " + group.ShowInMenu);
Console.WriteLine("Is Task Group Show Summary?: " + group.ShowSummary);
Console.WriteLine("Is Task Group should groups Assignments instead of Tasks?: " + group.GroupAssignments);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);
Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");

foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Task Criterion Field: " + criterion.Field);
    Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
    Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
    Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

    Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
    Console.WriteLine("Font Size: " + criterion.Font.Size);
    Console.WriteLine("Font Style: " + criterion.Font.Style);
    Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
}
```

### انظر أيضًا

* class [Group](../)
* namespace [Aspose.Tasks](../../group/)
* assembly [Aspose.Tasks](../../../)


