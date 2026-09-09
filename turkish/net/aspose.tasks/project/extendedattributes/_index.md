---
title: "Project.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. ExtendedAttributeDefinitionCollection nesnesini alır. Bir proje ile ilişkili genişletilmiş öznitelik özel alan tanımlarının koleksiyonu"
type: docs
weight: 410
url: /tr/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

ExtendedAttributeDefinitionCollection nesnesini alır. Bu nesne, bir proje ile ilişkili genişletilmiş öznitelik (özel alanlar) tanımlarının koleksiyonudur.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Örnekler

Genişletilmiş özniteliklerle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Custom alanı proje içinde yoksa, oluşturun.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Tanımdan Extended Attribute oluştur
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Göreve genişletilmiş öznitelik ekle
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


