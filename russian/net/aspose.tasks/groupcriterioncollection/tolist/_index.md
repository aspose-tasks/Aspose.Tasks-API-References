---
title: "GroupCriterionCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "GroupCriterionCollection метод. Преобразует коллекцию GroupCriterion в список объектов GroupCriterion"
type: docs
weight: 90
url: /ru/net/aspose.tasks/groupcriterioncollection/tolist/
---
## GroupCriterionCollection.ToList method

Преобразует коллекцию GroupCriterion в список объектов [`GroupCriterion`](../../groupcriterion/).

```csharp
public List<GroupCriterion> ToList()
```

### Возвращаемое значение

Обобщённый список объектов [`GroupCriterion`](../../groupcriterion/).

## Примеры

Показывает, как работать с коллекцией критериев группы.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// перебор критериев группы
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

// копировать критерии в другую группу
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### См. также

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


