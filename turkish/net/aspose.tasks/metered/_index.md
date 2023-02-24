---
title: Class Metered
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.Metered sınıf. Ölçülen anahtarı ayarlamak için yöntemler sağlar.
type: docs
weight: 890
url: /tr/net/aspose.tasks/metered/
---
## Metered class

Ölçülen anahtarı ayarlamak için yöntemler sağlar.

```csharp
public class Metered
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Metered](metered/)() | Default_Constructor |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Önceki kurulum lisansını kaldırır. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Tarifeli genel ve özel anahtarları ayarlar. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Tüketim kredisi alır. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Tüketim dosyası boyutunu alır. |

### Örnekler

Bu örnekte, ölçülü genel ve özel anahtar ayarlanmaya çalışılacaktır.

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

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks/)
* toplantı [Aspose.Tasks](../../)


