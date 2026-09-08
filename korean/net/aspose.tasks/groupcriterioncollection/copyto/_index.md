---
title: "GroupCriterionCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GroupCriterionCollection 메서드. 이 컬렉션의 요소들을 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/groupcriterioncollection/copyto/
---
## GroupCriterionCollection.CopyTo method

이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다.

```csharp
public void CopyTo(GroupCriterion[] array, int arrayIndex)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 배열 | GroupCriterion[] | 요소를 복사할 지정된 1차원 배열. |
| arrayIndex | Int32 | 복사가 시작되는 지정된 배열의 0 기반 인덱스. |

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

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


