---
title: "Project.RenumberWBSCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. إعادة ترقيم رمز WBS لجميع المهام"
type: docs
weight: 1180
url: /ar/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

إعادة ترقيم رمز WBS لجميع المهام.

```csharp
public void RenumberWBSCode()
```

## الأمثلة

يظهر كيفية إعادة ترقيم رموز WBS للمهام.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// الإخراج: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// الإخراج: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

إعادة ترقيم رمز WBS للمهام التي تم تمريرها.

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| taskIds | List`1 | معرفات المهام لإعادة ترقيم رموز WBS. |

## الأمثلة

يظهر كيفية إعادة ترقيم رموز WBS للمهام المحددة.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// الإخراج: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// الإخراج: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


