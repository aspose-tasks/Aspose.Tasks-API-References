---
title: "클래스 GroupCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GroupCollection 클래스. Group 객체 목록을 포함합니다. ICollectionGroup 인터페이스를 구현합니다."
type: docs
weight: 780
url: /ko/net/aspose.tasks/groupcollection/
---
## GroupCollection class

[`Group`](../group/) 객체 목록을 포함합니다. Implements ICollection&lt;Group&gt; 인터페이스.

```csharp
public class GroupCollection : ICollection<Group>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | 그룹 컬렉션을 [`Group`](../group/) 객체 목록으로 변환합니다. |

## 예제

그룹 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// 작업 그룹을 반복합니다
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// 리소스 그룹을 반복합니다
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// 다른 프로젝트의 그룹을 지웁니다
otherProject.TaskGroups.Clear();

// 그룹을 다른 프로젝트에 복사합니다
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// 사용자 정의 작업 그룹을 추가합니다
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

// 모든 그룹을 제거합니다
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### 또 보기

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


