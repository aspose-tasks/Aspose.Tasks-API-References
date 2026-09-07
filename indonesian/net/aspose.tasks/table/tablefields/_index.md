---
title: "Table.TableFields"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Table property. Gets a TableFields collection representing the fields in the table"
type: docs
weight: 90
url: /id/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Mendapatkan koleksi TableFields yang mewakili bidang-bidang dalam tabel.

```csharp
public TableFieldCollection TableFields { get; }
```

## Contoh

Shows how to work project's tables.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Define new custom attribute
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Add custom text attribute to created task.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Sesuaikan tabel dengan menambahkan bidang atribut teks
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

### Lihat Juga

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


