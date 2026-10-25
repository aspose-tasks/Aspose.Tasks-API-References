---
title: "GroupCriterionCollection.Remove"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GroupCriterionCollection 메서드. 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/groupcriterioncollection/remove/
---
## GroupCriterionCollection.Remove method

이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다.

```csharp
public bool Remove(GroupCriterion item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | GroupCriterion | 제거할 지정된 객체. |

### 반환 값

지정된 객체가 이 컬렉션에서 성공적으로 제거되면 true; 그렇지 않으면 false.

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


