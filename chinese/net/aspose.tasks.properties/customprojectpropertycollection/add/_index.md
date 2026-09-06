---
title: "CustomProjectPropertyCollection.Add"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CustomProjectPropertyCollection 方法。创建一个新的自定义属性。"
type: docs
weight: 30
url: /zh/net/aspose.tasks.properties/customprojectpropertycollection/add/
---
## Add(string, string) {#add_3}

创建一个新的自定义属性。

```csharp
public CustomProjectProperty Add(string name, string value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | 字符串 | 属性的名称。 |
| value | 字符串 | 新创建的属性对象值。 |

### 返回值

新创建的属性对象。

## 示例

展示如何使用自定义项目属性集合。

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// 让我们添加新的自定义属性
// 集合支持 Boolean、DateTime、Double、String 类型
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// 自定义属性可通过类型化集合访问
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// 获取自定义属性值
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// 遍历自定义属性的名称
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// 可以通过字符串键删除值
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// 或者可以完全清除集合
project.CustomProps.Clear();
```

### 另见

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, bool) {#add}

创建一个新的自定义属性。

```csharp
public CustomProjectProperty Add(string name, bool value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | 字符串 | 属性的名称。 |
| value | Boolean | 新创建的属性对象值。 |

### 返回值

新创建的属性对象。

## 示例

展示如何使用自定义项目属性集合。

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// 让我们添加新的自定义属性
// 集合支持 Boolean、DateTime、Double、String 类型
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// 自定义属性可通过类型化集合访问
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// 获取自定义属性值
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// 遍历自定义属性的名称
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// 可以通过字符串键删除值
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// 或者可以完全清除集合
project.CustomProps.Clear();
```

### 另见

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, double) {#add_1}

创建一个新的自定义属性。

```csharp
public CustomProjectProperty Add(string name, double value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | 字符串 | 属性的名称。 |
| value | Double | 新创建的属性对象值。 |

### 返回值

新创建的属性对象。

## 示例

展示如何使用自定义项目属性集合。

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// 让我们添加新的自定义属性
// 集合支持 Boolean、DateTime、Double、String 类型
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// 自定义属性可通过类型化集合访问
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// 获取自定义属性值
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// 遍历自定义属性的名称
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// 可以通过字符串键删除值
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// 或者可以完全清除集合
project.CustomProps.Clear();
```

### 另见

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, DateTime) {#add_2}

创建一个新的自定义属性。

```csharp
public CustomProjectProperty Add(string name, DateTime value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | 字符串 | 属性的名称。 |
| value | DateTime | 新创建的属性对象值。 |

### 返回值

新创建的属性对象。

## 示例

展示如何使用自定义项目属性集合。

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// 让我们添加新的自定义属性
// 集合支持 Boolean、DateTime、Double、String 类型
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// 自定义属性可通过类型化集合访问
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// 获取自定义属性值
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// 遍历自定义属性的名称
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// 可以通过字符串键删除值
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// 或者可以完全清除集合
project.CustomProps.Clear();
```

### 另见

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


