---
title: ExtendedAttributeDefinition.CreateExtendedAttribute
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition method. Creates a new extended attribute with the field ID which equals to this objects field ID value
type: docs
weight: 310
url: /net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Creates a new extended attribute with the field ID which equals to this object's field ID value.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute/) class with the fieldID which equals to this object's fieldID value.

## Examples

Shows how to create extended attributes.

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified text value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| textValue | String | The specified text value. |

### Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute/) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype/) is not 'Text' |

## Examples

Shows how to create extended attribute definition and set a string value of the attribute while its constructing.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// create extended attribute with a value equals to the 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// add extended attribute initialized by value the 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### See Also

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified numeric value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| numericValue | Decimal | The specified numeric value. |

### Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute/) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype/) is not 'Number' or 'Cost' |

## Examples

Shows how to create extended attribute definition and set a decimal value of the attribute while its constructing.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// create extended attribute with a value equals to 999m 
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// add extended attribute initialized by value 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### See Also

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified date value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dateTimeValue | DateTime | The specified date time value. |

### Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute/) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype/) is not 'Date', 'Start' or 'Finish' |

## Examples

Shows how to create extended attribute definition and set a datetime value of the attribute while its constructing.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// create extended attribute with a value equals to DateTime.Now 
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// add extended attribute
task.ExtendedAttributes.Add(extendedAttribute);
```

### See Also

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| durationValue | Duration | The specified duration value. |

### Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute/) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype/) is not 'Duration' |

## Examples

Shows how to create extended attribute definition and set a duration while its constructing.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// extended attribute Duration1 = 2 days
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// add extended attribute to the task
task.ExtendedAttributes.Add(extendedAttribute);
```

### See Also

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| flagValue | Boolean | The specified flag value. |

### Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute/) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype/) is not 'Flag' |

## Examples

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Creates new extended attribute linked with specified [`Value`](../../value/) item.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| lookupValue | Value | The specified [`Value`](../../value/) item. |

### Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute/) class linked with specified [`Value`](../../value/) item.

## Remarks

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Examples

Use this code to create new [`ExtendedAttribute`](../../extendedattribute/) using specific value:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Shows how to create extended attribute definition and set a value while its constructing.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Create a custom field definition based on the lookup table, which was declared above.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// create extended attribute for a value 
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// add extended attribute to the task
task.ExtendedAttributes.Add(extendedAttribute);
```

### See Also

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


