---
title: "Table.TableFields"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Table प्रॉपर्टी। टेबल में फ़ील्ड्स का प्रतिनिधित्व करने वाली TableFields कलेक्शन प्राप्त करता है"
type: docs
weight: 90
url: /hi/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

टेबल में फ़ील्ड्स को दर्शाने वाला TableFields कलेक्शन प्राप्त करता है।

```csharp
public TableFieldCollection TableFields { get; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट की टेबल्स के साथ कैसे काम किया जाए।

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// नया कस्टम एट्रिब्यूट परिभाषित करें
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// बनाए गए टास्क में कस्टम टेक्स्ट एट्रिब्यूट जोड़ें।
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// टेबल को कस्टमाइज़ करें टेक्स्ट एट्रिब्यूट फ़ील्ड जोड़कर
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

### संबंधित देखें

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


