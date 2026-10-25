---
title: "Project.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取 ExtendedAttributeDefinitionCollection 对象。该集合是与项目关联的扩展属性自定义字段定义的集合"
type: docs
weight: 410
url: /zh/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

获取 ExtendedAttributeDefinitionCollection 对象。该集合包含与项目关联的扩展属性（自定义字段）定义。

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## 示例

展示如何使用扩展属性。

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

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


