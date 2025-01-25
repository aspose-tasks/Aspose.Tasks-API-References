---
title: Table.TableFields
second_title: Aspose.Tasks for .NET API Reference
description: Table property. Gets a TableFields collection representing the fields in the table
type: docs
weight: 90
url: /net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Gets a TableFields collection representing the fields in the table.

```csharp
public TableFieldCollection TableFields { get; }
```

## Examples

Shows how to work project's tables.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Define new custom attribute
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Add custom text attribute to created task.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Customize table by adding text attribute field
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### See Also

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


