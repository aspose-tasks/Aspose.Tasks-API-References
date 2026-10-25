---
title: "类 GroupCriterionCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GroupCriterionCollection 类。包含一组 GroupCriterion 对象。实现 ICollectionGroupCriterion 接口。"
type: docs
weight: 800
url: /zh/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

包含一个 [`GroupCriterion`](../groupcriterion/) 对象的集合。实现 ICollection&lt;GroupCriterion&gt; 接口。

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | 从此集合中移除特定对象的第一次出现。 |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | 将 GroupCriterion 集合转换为 [`GroupCriterion`](../groupcriterion/) 对象的列表。 |

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

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


