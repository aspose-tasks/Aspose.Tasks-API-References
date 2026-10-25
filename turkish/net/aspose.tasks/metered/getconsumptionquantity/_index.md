---
title: "Metered.GetConsumptionQuantity"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Metered yöntemi. Tüketim dosya boyutunu alır"
type: docs
weight: 60
url: /tr/net/aspose.tasks/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Tüketim dosya boyutunu alır.

```csharp
public static decimal GetConsumptionQuantity()
```

### Dönüş Değeri

Tüketilen bayt sayısını döndürür.

## Örnekler

Aspose.Tasks ile &lt;see cref=\"Aspose.Tasks.Metered\" /&gt; lisans türünün nasıl kullanılacağını gösterir.

```csharp
// Ölçümlü lisansı kullanalım (bkz. https://purchase.aspose.com/faqs/licensing/metered)
// ölçümlü lisansı ayarla
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// projeyle çalış...
// ...

// Mevcut kredileri ve bayt tüketimini alabiliriz.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // istisna kaydet
}

// son zamanlarda kullanıcı bir ölçümlüyü sıfırlayabilir ve bayt sayımını durdurabilir
metered.ResetMeteredKey();
```

### Ayrıca Bakınız

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


