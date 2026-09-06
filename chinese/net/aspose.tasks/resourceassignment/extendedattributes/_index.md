---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 属性。获取或设置此对象的 ExtendedAttributeCollection 类实例"
type: docs
weight: 250
url: /zh/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

获取或设置此对象的 ExtendedAttributeCollection 类的实例。

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## 备注

仅支持 XML 格式的读取。

## 示例

展示如何为分配添加扩展属性。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 通过创建 ResourceAssignment 对象，将资源 "1 TRG: Trade Group" 分配给 "TASK 1"。
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// 创建带查找的自定义属性定义。
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// 此值可在 MS Project 的 "Resource usage" 视图中看到。
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### 另见

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


