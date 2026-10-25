---
title: "FilterCriteria.CriteriaRows"
second_title: "Aspose.Tasks for .NET API 参考"
description: "FilterCriteria 属性。获取子 FilterCriteria 行的列表。如果过滤器包含多个标准行，则 And 运算符的效果是必须同时满足两行的标准，任务或资源才会作为此过滤器的结果显示。Or 运算符的效果是只需满足其中一行的标准即可。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/filtercriteria/criteriarows/
---
## FilterCriteria.CriteriaRows property

获取子 [`FilterCriteria`](../) 行的列表。如果过滤器包含多个标准行，则 And 运算符的效果是必须同时满足两行的标准，任务或资源才会作为此过滤器的结果显示。Or 运算符的效果是只需满足其中一行的标准即可。

```csharp
public List<FilterCriteria> CriteriaRows { get; }
```

## 示例

展示如何读取任务过滤条件。

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// 将过滤条件打印为字符串
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### 另见

* class [FilterCriteria](../)
* namespace [Aspose.Tasks](../../filtercriteria/)
* assembly [Aspose.Tasks](../../../)


