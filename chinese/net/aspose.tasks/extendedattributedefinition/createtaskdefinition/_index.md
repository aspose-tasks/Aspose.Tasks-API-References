---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttributeDefinition 方法。工厂方法，用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 None。其 CalculationType 等于 None，并且只能在任务中使用。调用此方法时需要指定 customFieldType、fieldId 和 alias。"
type: docs
weight: 40
url: /zh/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

工厂方法，用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 "None"。它的 [`CalculationType`](../calculationtype/) 等于 None，并且只能在任务中使用。调用此方法时需要指定 *customFieldType*、*fieldId* 和 *alias*。

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| customFieldType | CustomFieldType | 指定的 [`CustomFieldType`](../../customfieldtype/) 类型。 |
| fieldId | ExtendedAttributeTask | 指定的[`ExtendedAttributeTask`](../../extendedattributetask/)字段 ID。 |
| 别名 | 字符串 | 指定的 String 别名。 |

### 返回值

已创建带有指定 *customFieldType*、*fieldId* 和 *alias* 的 [`ExtendedAttributeDefinition`](../) 类实例。

## 示例

使用此示例创建自定义文本字段定义：

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

展示如何创建任务的扩展属性。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 创建 Text1 类型的扩展属性定义
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// 将其添加到项目的扩展属性集合
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// 向项目添加任务
var task = project.RootTask.Children.Add("Task 1");

// 从属性定义创建扩展属性
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// 为生成的扩展属性分配值。该属性的类型为 "Text"，应使用 "TextValue" 属性。
taskExtendedAttributeText1.TextValue = "London";

// 将扩展属性添加到任务
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// 创建 Text2 类型的扩展属性定义
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// 为扩展属性定义添加查找值。
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// 将其添加到项目的扩展属性集合
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// 向项目添加任务
var task2 = project4.RootTask.Children.Add("Task 2");

// 从 Text2 查找定义（ID 为 1）创建扩展属性
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// 将扩展属性添加到任务
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// 创建 Duration2 类型的扩展属性定义
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// 为扩展属性定义添加查找值
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// 将该定义添加到项目的扩展属性集合
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// 向项目添加任务
var task3 = project2.RootTask.Children.Add("Task 3");

// 从 Duration2 查找定义（ID 为 3）创建扩展属性
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// 将扩展属性添加到任务
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// 创建 Finish2 类型的扩展属性定义
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// 为扩展属性定义添加查找值
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// 将该定义添加到项目的扩展属性集合
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// 向项目添加任务
var task4 = project3.RootTask.Children.Add("Task 4");

// 从 Finish2 查找定义（ID 为 3）创建扩展属性
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// 将扩展属性添加到任务
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

工厂方法用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 "None"。它的 [`CalculationType`](../calculationtype/) 等于 None，并且只能在任务中使用。调用此方法时需要指定 *fieldId* 和 *alias*。字段类型从字段 ID 推断。

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | 指定的[`ExtendedAttributeTask`](../../extendedattributetask/)字段 ID。 |
| 别名 | 字符串 | 指定的 String 别名。 |

### 返回值

已创建带有指定 *fieldId* 和 *alias* 的 [`ExtendedAttributeDefinition`](../) 类实例。

## 示例

使用此示例创建自定义文本字段定义：

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

展示如何创建扩展属性定义并在构建时设置属性的字符串值。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 创建扩展属性，值等于 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// 添加已使用值 'Common Info' 初始化的扩展属性
task.ExtendedAttributes.Add(extendedAttribute);
```

### 另见

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


