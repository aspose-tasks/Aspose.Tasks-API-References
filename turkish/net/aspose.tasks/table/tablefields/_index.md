---
title: "Table.TableFields"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Table özelliği. Tablo içindeki alanları temsil eden bir TableFields koleksiyonunu alır"
type: docs
weight: 90
url: /tr/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Tablodaki alanları temsil eden bir TableFields koleksiyonunu alır.

```csharp
public TableFieldCollection TableFields { get; }
```

## Örnekler

Projenin tablolarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Yeni özel öznitelik tanımla
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Oluşturulan göreve özel metin özniteliği ekle.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Tabloyu metin özelliği alanı ekleyerek özelleştirin
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

### Ayrıca Bakınız

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


