---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Metered yöntemi. Metered genel ve özel anahtarları ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Ölçülen genel ve özel anahtarları ayarlar.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| publicKey | Dize | Açık anahtar. |
| privateKey | Dize | Özel anahtar. |

## Açıklamalar

Eğer metered lisansı satın alırsanız, bu API uygulama başlangıcında çağrılmalıdır; genellikle bu yeterlidir. Ancak, metered 24 saat içinde tüketim verilerini yükleyemezse, lisans değerlendirme durumuna ayarlanır. Böyle bir durumu önlemek için lisans durumunu düzenli olarak kontrol etmelisiniz. Eğer değerlendirme durumundaysa, bu API'yi tekrar çağırın.

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


