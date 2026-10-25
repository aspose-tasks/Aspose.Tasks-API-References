---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition yöntemi. ExtendedAttributeDefinition sınıfının örneği için bir karma kodu döndürür."
type: docs
weight: 330
url: /tr/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

[`ExtendedAttributeDefinition`](../) sınıfının örneği için bir karma kodu döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kodu.

## Örnekler

Genişletilmiş bir öznitelik tanımının karma kodunu nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// Genişletilmiş bir öznitelik tanımının karma kodu bir alan kimliğine eşittir.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### Ayrıca Bakınız

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


