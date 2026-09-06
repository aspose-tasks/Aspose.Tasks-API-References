---
title: "枚举 FilterOperation"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.FilterOperation 枚举。指定使用 FieldName、FilterComparisonType 和 Value 建立的条件如何与过滤器中的其他条件关联"
type: docs
weight: 640
url: /zh/net/aspose.tasks/filteroperation/
---
## FilterOperation enumeration

指定使用 FieldName、FilterComparisonType 和 Value 建立的准则如何与过滤器中的其他准则关联。

```csharp
public enum FilterOperation
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `0` | 未定义。 |
| And | `1` | AND 运算符。 |
| Or | `2` | OR 运算符。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


