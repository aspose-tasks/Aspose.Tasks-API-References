---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment özelliği. Bu nesne için ExtendedAttributeCollection sınıfının bir örneğini alır veya ayarlar"
type: docs
weight: 250
url: /tr/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Bu nesne için ExtendedAttributeCollection sınıfının bir örneğini alır veya ayarlar.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Açıklamalar

Okuma yalnızca XML biçimi için desteklenir.

## Örnekler

Bir atama için genişletilmiş özniteliklerin nasıl ekleneceğini gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// ResourceAssignment nesnesi oluşturarak "1 TRG: Trade Group" kaynağını "TASK 1" görevine atayın.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Aramayı içeren özel öznitelik tanımı oluştur.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// Bu değer, MS Project'in "Resource usage" görünümünde görülebilir.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### Ayrıca Bakınız

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


