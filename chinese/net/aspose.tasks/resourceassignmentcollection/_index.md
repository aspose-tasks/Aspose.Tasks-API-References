---
title: "类 ResourceAssignmentCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ResourceAssignmentCollection 类。表示 ResourceAssignment 对象的集合"
type: docs
weight: 1760
url: /zh/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

表示一个 [`ResourceAssignment`](../resourceassignment/) 对象的集合。

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | 获取 ResourceAssignmentCollection 中包含的对象数量。 |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读。 |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | 返回指定索引处的元素。 |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | 获取 ResourceAssignmentCollection 对象的父项目。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | 这是 ICollection 的 Add 方法的存根实现，只会抛出 NotSupportedException。 |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | 向 ResourceAssignmentCollection 添加新分配。 |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | 向 ResourceAssignmentCollection 添加新分配。 |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | 向 ResourceAssignmentCollection 添加新分配。 |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | 返回具有指定 uid 的分配。 |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | 从集合中移除指定的分配（如果集合不是只读的），否则抛出 NotSupportedException。 |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | 移除指定索引处的分配（如果集合不是只读的），否则抛出 NotSupportedException。 |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | 将 ResourceAssignmentCollection 对象转换为 [`ResourceAssignment`](../resourceassignment/) 对象的列表。 |

## 示例

展示如何使用资源分配集合。

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

// 处理分配...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// 将集合转换为列表
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// 遍历列表
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### 另见

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


