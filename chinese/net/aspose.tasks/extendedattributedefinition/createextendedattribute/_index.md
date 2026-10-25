---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttributeDefinition 方法。创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值"
type: docs
weight: 310
url: /zh/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值。

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### 返回值

返回已创建的 [`ExtendedAttribute`](../../extendedattribute/) 类实例，其 fieldID 等于此对象的 fieldID 值。

## 示例

展示如何创建扩展属性。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// 如果项目中不存在自定义字段，则创建它。
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// 从定义生成扩展属性
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// 向任务添加扩展属性
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的文本值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| textValue | 字符串 | 指定的文本值。 |

### 返回值

返回已创建的 [`ExtendedAttribute`](../../extendedattribute/) 类实例，其 fieldID 等于此对象的 fieldID 值。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 如果当前 [`CfType`](../cftype/) 不是 'Text' |

## 示例

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的数值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| numericValue | Decimal | 指定的数值。 |

### 返回值

返回已创建的 [`ExtendedAttribute`](../../extendedattribute/) 类实例，其 fieldID 等于此对象的 fieldID 值。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 如果当前 [`CfType`](../cftype/) 不是 'Number' 或 'Cost' |

## 示例

展示如何创建扩展属性定义并在构建时设置属性的十进制值。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 创建扩展属性，值等于 999m
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// 添加已使用值 999m 初始化的扩展属性
task.ExtendedAttributes.Add(extendedAttribute);
```

### 另见

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的日期值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dateTimeValue | DateTime | 指定的日期时间值。 |

### 返回值

返回已创建的 [`ExtendedAttribute`](../../extendedattribute/) 类实例，其 fieldID 等于此对象的 fieldID 值。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 如果当前 [`CfType`](../cftype/) 不是 'Date'、'Start' 或 'Finish' |

## 示例

展示如何创建扩展属性定义并在构建时设置属性的日期时间值。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 创建扩展属性，其值等于 DateTime.Now
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// 添加扩展属性
task.ExtendedAttributes.Add(extendedAttribute);
```

### 另见

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的持续时间值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| durationValue | 持续时间 | 指定的持续时间值。 |

### 返回值

返回已创建的 [`ExtendedAttribute`](../../extendedattribute/) 类实例，其 fieldID 等于此对象的 fieldID 值。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 如果当前 [`CfType`](../cftype/) 不是 'Duration' |

## 示例

展示如何创建扩展属性定义并在构建时设置持续时间。

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// 扩展属性 Duration1 = 2 天
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// 向任务添加扩展属性
task.ExtendedAttributes.Add(extendedAttribute);
```

### 另见

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的标志值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| flagValue | Boolean | 指定的标志值。 |

### 返回值

返回已创建的 [`ExtendedAttribute`](../../extendedattribute/) 类实例，其 fieldID 等于此对象的 fieldID 值。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 如果当前 [`CfType`](../cftype/) 不是 'Flag' |

## 示例

展示如何创建扩展属性定义并在构建时设置标志的值。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// 为布尔自定义字段创建定义
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// 创建属性并将初始值设为 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### 另见

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

创建与指定的 [`Value`](../../value/) 项关联的新扩展属性。

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| lookupValue | Value | 指定的 [`Value`](../../value/) 项。 |

### 返回值

返回已创建的与指定的 [`Value`](../../value/) 项关联的 [`ExtendedAttribute`](../../extendedattribute/) 类实例。

## 备注

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## 示例

使用以下代码通过特定值创建新的 [`ExtendedAttribute`](../../extendedattribute/)：

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

展示如何创建扩展属性定义并在构建时设置值。

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 基于上面声明的查找表创建自定义字段定义。
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// 为值创建扩展属性
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// 向任务添加扩展属性
task.ExtendedAttributes.Add(extendedAttribute);
```

### 另见

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


