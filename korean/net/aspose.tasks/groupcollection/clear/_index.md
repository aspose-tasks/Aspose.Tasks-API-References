---
title: "GroupCollection.Clear"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GroupCollection 메서드. 이 컬렉션의 모든 항목을 제거합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/groupcollection/clear/
---
## GroupCollection.Clear method

이 컬렉션에서 모든 항목을 제거합니다.

```csharp
public void Clear()
```

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

* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


