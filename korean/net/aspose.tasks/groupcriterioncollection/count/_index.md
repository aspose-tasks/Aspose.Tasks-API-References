---
title: "GroupCriterionCollection.Count"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GroupCriterionCollection 속성. 이 컬렉션에 포함된 요소 수를 가져옵니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/groupcriterioncollection/count/
---
## GroupCriterionCollection.Count property

이 컬렉션에 포함된 요소 수를 가져옵니다.

```csharp
public int Count { get; }
```

## 예제

그룹 기준 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// 그룹 기준을 반복합니다
Console.WriteLine("Print group criteria of the group '{0}': ", group.Name);
Console.WriteLine("Group criterion count: " + group.GroupCriteria.Count);
foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Field: " + criterion.Field);
    Console.WriteLine("Group On: " + criterion.GroupOn);
    Console.WriteLine();
}

group.GroupCriteria.Clear();

if (!group.GroupCriteria.IsReadOnly)
{
    List<GroupCriterion> groupCriteria = group.GroupCriteria.ToList();
    foreach (var criterion in groupCriteria)
    {
        group.GroupCriteria.Remove(criterion);
    }
}

var criterionToAdd = new GroupCriterion
{
    Ascending = true,
    Field = Field.TaskActive
};

if (!group.GroupCriteria.Contains(criterionToAdd))
{
    group.GroupCriteria.Add(criterionToAdd);
}

// 기준을 다른 그룹에 복사합니다
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### 또 보기

* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


