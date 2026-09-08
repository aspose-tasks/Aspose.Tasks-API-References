---
title: "클래스 GroupCriterionCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GroupCriterionCollection 클래스. GroupCriterion 객체의 컬렉션을 포함합니다. ICollectionGroupCriterion 인터페이스를 구현합니다."
type: docs
weight: 800
url: /ko/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

[`GroupCriterion`](../groupcriterion/) 객체의 컬렉션을 포함합니다. ICollection&lt;GroupCriterion&gt; 인터페이스를 구현합니다.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | GroupCriterion 컬렉션을 [`GroupCriterion`](../groupcriterion/) 객체 목록으로 변환합니다. |

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

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


