---
title: "GroupCriterionCollection.ToList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GroupCriterionCollection 方法。将 GroupCriterion 集合转换为 GroupCriterion 对象的列表"
type: docs
weight: 90
url: /zh/net/aspose.tasks/groupcriterioncollection/tolist/
---
## GroupCriterionCollection.ToList method

将 GroupCriterion 集合转换为 [`GroupCriterion`](../../groupcriterion/) 对象的列表。

```csharp
public List<GroupCriterion> ToList()
```

### 返回值

[`GroupCriterion`](../../groupcriterion/) 对象的通用列表。

## 示例

展示如何使用分组标准的集合。

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// 遍历分组标准
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

// 将标准复制到其他组
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### 另见

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


