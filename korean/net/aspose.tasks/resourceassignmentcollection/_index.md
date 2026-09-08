---
title: "클래스 ResourceAssignmentCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ResourceAssignmentCollection 클래스. ResourceAssignment 개체의 컬렉션을 나타냅니다."
type: docs
weight: 1760
url: /ko/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

[`ResourceAssignment`](../resourceassignment/) 개체의 컬렉션을 나타냅니다.

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | ResourceAssignmentCollection에 포함된 개체 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | 지정된 인덱스의 요소를 반환합니다. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | ResourceAssignmentCollection 객체의 상위 프로젝트를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | ICollection의 Add 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | ResourceAssignmentCollection에 새 할당을 추가합니다. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | ResourceAssignmentCollection에 새 할당을 추가합니다. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | ResourceAssignmentCollection에 새 할당을 추가합니다. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | 지정된 uid를 가진 할당을 반환합니다. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | 컬렉션이 읽기 전용이 아닌 경우 지정된 할당을 컬렉션에서 제거하고, 읽기 전용인 경우 NotSupportedException을 throw합니다. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | 컬렉션이 읽기 전용이 아닌 경우 지정된 인덱스의 할당을 제거하고, 읽기 전용인 경우 NotSupportedException을 throw합니다. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | ResourceAssignmentCollection 객체를 [`ResourceAssignment`](../resourceassignment/) 개체 목록으로 변환합니다. |

## 예제

리소스 할당 컬렉션 작업 방법을 보여줍니다.

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

// 할당 작업...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// 컬렉션을 리스트로 변환합니다
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// 리스트를 반복합니다
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### 또 보기

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


