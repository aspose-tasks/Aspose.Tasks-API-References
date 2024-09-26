---
title: ExtendedAttributeDefinition.CreateResourceDefinition
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition method. Factory method which creates a simple extended attribute definition which Microsoft Project shows as None. It has CalculationType equals to None and can be used in Resource only. You are required to specify customFieldType fieldId and alias when call this method
type: docs
weight: 30
url: /net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](../calculationtype/) equals to None and can be used in Resource only. You are required to specify *customFieldType*, *fieldId* and *alias* when call this method.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | CustomFieldType | The specified [`CustomFieldType`](../../customfieldtype/) type. |
| fieldId | ExtendedAttributeResource | The specified [`ExtendedAttributeResource`](../../extendedattributeresource/) field ID. |
| alias | String | The specified String alias. |

### Return Value

Created instance of the [`ExtendedAttributeDefinition`](../) class with specified *customFieldType*, *fieldId* and *alias*.

## Examples

Use this example to create a custom text field definition:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Shows how to add extended attribute to a resource assignment.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Add new task and resource
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // Custom attributes which is visible in "Resource Usage" view can be created with ExtendedAttributeDefinition.CreateResourceDefinition method.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // The type of the attribute is "Cost", so we need to use "NumericValue" property.
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // Custom attributes which is visible in "Task Usage" view can be created with ExtendedAttributeDefinition.CreateTaskDefinition method
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // The type of the attribute is "Cost", so we need to use "NumericValue" property.
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](../calculationtype/) equals to None and can be used in Resource only. You are required to specify *fieldId* and *alias* when call this method. The field type is inferred from field id.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | The specified [`ExtendedAttributeResource`](../../extendedattributeresource/) field ID. |
| alias | String | The specified String alias. |

### Return Value

Created instance of the [`ExtendedAttributeDefinition`](../) class with specified *fieldId* and *alias*.

## Examples

Use this example to create a custom text field definition:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Shows how to create extended attribute definition and set a value of a flag while its constructing.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// create a definition for a boolean custom field
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// create an attribute and set the initial value to 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### See Also

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


