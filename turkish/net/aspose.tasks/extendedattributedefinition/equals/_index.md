---
title: "ExtendedAttributeDefinition.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition yöntemi. Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür"
type: docs
weight: 320
url: /tr/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | bu örnek ile karşılaştırılacak belirtilen nesne. |

### Dönüş Değeri

bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak.

## Örnekler

Genişletilmiş öznitelik tanımının eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// Takvimlerin eşitliği, öznitelik tanımı alan kimliklerine karşı kontrol edilir.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### Ayrıca Bakınız

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


