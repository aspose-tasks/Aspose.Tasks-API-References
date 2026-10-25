---
title: "Sınıf Metered"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Metered sınıfı. Ölçülen anahtarı ayarlamak için yöntemler sağlar"
type: docs
weight: 1020
url: /tr/net/aspose.tasks/metered/
---
## Metered class

Ölçülü anahtarı ayarlamak için yöntemler sağlar.

```csharp
public class Metered
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Metered](metered/)() | Varsayılan yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Ürünün Ölçülen lisans kullanılarak başarılı bir şekilde lisanslanıp lisanslanmadığını kontrol eder. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Daha önce ayarlanmış lisansı kaldırır. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Ölçülen genel ve özel anahtarları ayarlar. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Tüketim kredisini alır. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Tüketim dosya boyutunu alır. |

## Örnekler

Bu örnekte, ölçülen genel ve özel anahtarı ayarlamaya çalışılacak

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

bileşen jar dosyası:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


