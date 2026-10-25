---
title: "枚举 FilterComparisonType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.FilterComparisonType 枚举。 在过滤器或图形指示器中，用作选择条件的 FieldName 与 Value 之间的比较类型。"
type: docs
weight: 620
url: /zh/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

在 FieldName 与 Value 之间进行的比较类型，用作过滤器或图形指示器的选择条件。

```csharp
public enum FilterComparisonType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Equals | `6` | 字段 Field 的值等于 Value。 |
| DoesNotEqual | `7` | 字段 Field 的值不等于 Value。 |
| IsGreaterThan | `2` | 字段 Field 的值大于 Value。 |
| IsGreaterThanOrEqualTo | `4` | 字段 Field 的值大于或等于 Value。 |
| IsLessThan | `3` | 字段 Field 的值小于 Value。 |
| IsLessThanOrEqualTo | `5` | 字段 Field 的值小于或等于 Value。 |
| IsWithin | `1` | 字段 Field 的值在 Value 范围内。 |
| IsNotWithin | `9` | 字段 Field 的值不在 Value 范围内。 |
| Contains | `8` | 字段 Field 的值包含 Value。 |
| DoesNotContain | `10` | 字段 Field 的值不包含 Value。 |
| ContainsExactly | `11` | 字段 Field 的值完全包含 Value。 |
| IsOneOf | `12` | 字段 Field 的值等于指定的多个 Values 之一。用于自动筛选。 |
| Undefined | `0` | 未定义的值。 |
| IsAnyValue | `255` | “Is any value” 条件。适用于图形指示器。 |

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


