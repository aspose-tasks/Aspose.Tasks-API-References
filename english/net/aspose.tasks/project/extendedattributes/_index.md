---
title: Project.ExtendedAttributes
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets ExtendedAttributeDefinitionCollection object. The collection of extended attribute custom fields definitions associated with a project
type: docs
weight: 410
url: /net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

Gets ExtendedAttributeDefinitionCollection object. The collection of extended attribute (custom fields) definitions associated with a project.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Examples

Shows how to work with extended attributes.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// If the Custom field doesn't exist in Project, create it
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Generate Extended Attribute from definition
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Add extended attribute to task
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


