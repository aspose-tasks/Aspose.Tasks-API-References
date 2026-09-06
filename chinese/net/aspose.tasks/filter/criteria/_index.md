---
title: "Filter.Criteria"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Filter 属性。获取或设置任务或资源必须满足的条件，以在 MSP 视图中显示。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/filter/criteria/
---
## Filter.Criteria property

获取或设置任务或资源必须满足的条件，以在 MSP 视图中显示。

```csharp
public FilterCriteria Criteria { get; set; }
```

## 示例

展示如何读取任务过滤器。

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine(filter.Criteria.CriteriaRows.Count);
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine(criteria1.Test.ToString());
Console.WriteLine(criteria1.Field.ToString());
Console.WriteLine(criteria1.Values[0].ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine(criteria21.Test.ToString());
Console.WriteLine(criteria21.Field.ToString());
Console.WriteLine(criteria21.Values[0].ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine(criteria22.Test.ToString());
Console.WriteLine(criteria22.Field.ToString());
Console.WriteLine(criteria22.Values[0].ToString());
Console.WriteLine(filter.Criteria);
```

### 另见

* class [FilterCriteria](../../filtercriteria/)
* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


