---
title: "الفئة ResourceAssignmentCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ResourceAssignmentCollection. تمثل مجموعة من كائنات ResourceAssignment."
type: docs
weight: 1760
url: /ar/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

تمثل مجموعة من كائنات [`ResourceAssignment`](../resourceassignment/).

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | يحصل على عدد الكائنات الموجودة في ResourceAssignmentCollection. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | يحصل على المشروع الأب لكائن ResourceAssignmentCollection. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | هذا هو تنفيذ النموذج الأولي لطريقة Add في ICollection، والذي يرمي فقط NotSupportedException |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | يرجع تعيينًا بالمعرف الفريد المحدد. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | يزيل التعيين المحدد من المجموعة إذا لم تكن للقراءة فقط، وإلا يطرح استثناء NotSupportedException. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | يزيل التعيين عند الفهرس المحدد إذا لم تكن المجموعة للقراءة فقط، وإلا يطرح استثناء NotSupportedException. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | يحوّل كائن ResourceAssignmentCollection إلى قائمة من كائنات [`ResourceAssignment`](../resourceassignment/). |

## الأمثلة

يعرض كيفية العمل مع مجموعات تعيين الموارد.

```csharp
var project = new Project(DataDir + "TemplateResource2010.mpp");

var task = project.RootTask.Children.Add("Task 1");
var resource = project.Resources.Add("Resource 1");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignment.Set(Asn.Work, project.GetWork(40));
assignment.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

var assignmentWithUnits = project.ResourceAssignments.Add(task, resource, 1d);
assignmentWithUnits.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignmentWithUnits.Set(Asn.Work, project.GetWork(40));
assignmentWithUnits.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

var assignmentWithCost = project.ResourceAssignments.Add(task, resource);
assignmentWithCost.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignmentWithCost.Set(Asn.Work, project.GetWork(40));
assignmentWithCost.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

Console.WriteLine("Print assignments for the project: " + project.ResourceAssignments.ParentProject.Get(Prj.Name));
Console.WriteLine("Resource assignment count: " + project.ResourceAssignments.Count);
foreach (var resourceAssignment in project.ResourceAssignments)
{
    Console.WriteLine("Task Name: " + resourceAssignment.Get(Asn.Task).Get(Tsk.Name));
    Console.WriteLine("Uid: " + resourceAssignment.Get(Asn.Uid));
    Console.WriteLine("Start: " + resourceAssignment.Get(Asn.Start));
    Console.WriteLine("Work: " + resourceAssignment.Get(Asn.Work));
    Console.WriteLine("Finish: " + resourceAssignment.Get(Asn.Finish));
}

var assignmentByUid = project.ResourceAssignments.GetByUid(2);
Console.WriteLine("Assignment By Uid Start: " + assignmentByUid.Get(Asn.Start));

// العمل مع التعيين...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// تحويل المجموعة إلى قائمة
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// التكرار على القائمة
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### انظر أيضًا

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


