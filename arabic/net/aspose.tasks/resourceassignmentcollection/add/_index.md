---
title: "ResourceAssignmentCollection.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignmentCollection. يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection"
type: docs
weight: 50
url: /ar/net/aspose.tasks/resourceassignmentcollection/add/
---
## Add(Task, Resource, double) {#add_1}

يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource, double units)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | مهمة لتعيينها. |
| المورد | المورد | مورد لتعيينه. |
| الوحدات | Double | عدد الوحدات لتعيين جديد. |

### قيمة الإرجاع

تم إضافة التعيين.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Resource, decimal) {#add_2}

يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource, decimal cost)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | مهمة لتعيينها. |
| المورد | المورد | مورد تكلفة لتعيينه. |
| تكلفة | Decimal | تكلفة التعيين الجديد. |

### قيمة الإرجاع

تم إضافة التعيين.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Resource) {#add}

يضيف تعيينًا جديدًا إلى ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | مهمة لتعيينها. |
| المورد | المورد | مورد لتعيينه. |

### قيمة الإرجاع

تم إضافة التعيين.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(ResourceAssignment) {#add_3}

هذا هو تنفيذ النموذج الأولي لطريقة Add في ICollection، والذي يرمي فقط NotSupportedException

```csharp
public void Add(ResourceAssignment item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | ResourceAssignment | العنصر المراد إزالته. |

### انظر أيضًا

* class [ResourceAssignment](../../resourceassignment/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)


