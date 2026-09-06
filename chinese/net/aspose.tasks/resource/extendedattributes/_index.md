---
title: "Resource.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 属性。获取扩展属性的值"
type: docs
weight: 320
url: /zh/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

获取扩展属性的值。

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## 备注

需要两条数据——指向扩展属性表的指针（可通过唯一 ID 或字段 ID 指定），以及值（可直接指定值，或指向值列表的指针）。

## 示例

展示如何添加资源扩展属性。

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// 定义扩展属性
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// 创建扩展属性并设置其值
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// 添加新资源及其扩展属性
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


