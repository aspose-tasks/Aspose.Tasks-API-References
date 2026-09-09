---
title: "ExtendedAttribute.ToString"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttribute yöntemi. Genişletilmiş bir özniteliğin kısa dize temsilini döndürür"
type: docs
weight: 110
url: /tr/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Bir genişletilmiş özniteliğin kısa dize temsilini döndürür.

```csharp
public override string ToString()
```

### Dönüş Değeri

Genişletilmiş özniteliğin dize temsili.

## Örnekler

Genişletilmiş öznitelikleri okumanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Görevler için genişletilmiş öznitelikleri okuyun
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // genişletilmiş öznitelik hakkında ortak bilgileri oku
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


