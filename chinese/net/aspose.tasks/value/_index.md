---
title: "类 Value"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Value 类。表示值列表中的一个值"
type: docs
weight: 2800
url: /zh/net/aspose.tasks/value/
---
## Value class

表示值列表中的一个值。

```csharp
public class Value
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Value](value/)() | 初始化 `Value` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | 获取或设置实际值（如果可以表示为 DateTime）。默认值为 MinValue。 |
| [Description](../../aspose.tasks/value/description/) { get; set; } | 获取或设置值的描述。 |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | 获取或设置用于表示 Duration 的实际值。 |
| [Id](../../aspose.tasks/value/id/) { get; set; } | 获取或设置跨项目的值的唯一标识符。 |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | 获取或设置用于表示数字或成本值的实际值。 |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | 获取或设置自定义字段名称的拼音信息。 |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | 获取或设置用于表示文本字符串的实际值。 |
| [Val](../../aspose.tasks/value/val/) { get; set; } | 获取或设置内部表示中的实际值。建议使用下面列出的强类型属性。 |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | 获取一个 GUID，用于在整个项目中标识此值。 |

## 示例

展示如何读取并使用查找值。

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// 创建文本类型的扩展属性定义
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// 为扩展属性定义添加查找值。
textLookup.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1", Phonetic = "Town One" });
textLookup.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2", Phonetic = "Town Two" });

Console.WriteLine("Iterate over text lookup values:");
foreach (var value in textLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("String Value: " + value.StringValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// 创建持续时间类型的扩展属性定义。
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// 为扩展属性定义添加查找值。
durationLookup.AddLookupValue(new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours", Phonetic = "Four hours" });
durationLookup.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(8, TimeUnitType.Hour), Description = "1 day", Phonetic = "One day" });
durationLookup.AddLookupValue(new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour", Phonetic = "One hour" });
durationLookup.AddLookupValue(new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days", Phonetic = "Ten days" });

Console.WriteLine("Iterate over duration lookup values:");
foreach (var value in durationLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Duration: " + value.Duration);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// 创建日期类型的扩展属性定义。
var dateLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Date,
    ExtendedAttributeTask.Date1,
    "Custom Date");
dateLookup.AddLookupValue(new Value { Id = 7, DateTimeValue = new DateTime(2020, 4, 27, 8, 0, 0), Description = "Start Date", Phonetic = "Start Date" });

Console.WriteLine("Iterate over date lookup values:");
foreach (var value in dateLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("DateTime Value: " + value.DateTimeValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// 创建数字类型的扩展属性定义。
var numericLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Number,
    ExtendedAttributeTask.Number1,
    "Number of tons");
numericLookup.AddLookupValue(new Value { Id = 8, NumericValue = 10, Description = "10 tons", Phonetic = "Ten tons" });
numericLookup.AddLookupValue(new Value { Id = 9, NumericValue = 20, Description = "20 tons", Phonetic = "Twenty tons" });
numericLookup.AddLookupValue(new Value { Id = 10, NumericValue = 30, Description = "30 tons", Phonetic = "Thirty tons" });

Console.WriteLine("Iterate over numeric lookup values:");
foreach (var value in numericLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Numeric Value: " + value.NumericValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

project.ExtendedAttributes.Add(textLookup);
project.ExtendedAttributes.Add(durationLookup);
project.ExtendedAttributes.Add(dateLookup);
project.ExtendedAttributes.Add(numericLookup);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


