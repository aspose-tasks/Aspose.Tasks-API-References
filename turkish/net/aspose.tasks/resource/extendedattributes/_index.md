---
title: "Resource.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource özelliği. Uzatılmış bir niteliğin değerlerini alır."
type: docs
weight: 320
url: /tr/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Genişletilmiş bir niteliğin değerlerini alır.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Açıklamalar

İki veri parçası gereklidir - benzersiz kimlik ya da Alan kimliği ile belirtilen uzatılmış nitelik tablosuna geri işaret eden bir gösterge ve değeri ya doğrudan değerle ya da değer listesine geri işaret eden bir gösterge.

## Örnekler

Kaynak uzatılmış niteliklerin nasıl ekleneceğini gösterir.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Uzatılmış niteliği tanımla
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Genişletilmiş özniteliği oluştur ve değerini ayarla
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Yeni bir kaynak ekle ve onun genişletilmiş özniteliğini
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


