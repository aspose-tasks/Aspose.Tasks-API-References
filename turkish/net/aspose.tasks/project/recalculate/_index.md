---
title: Project.Recalculate
second_title: Aspose.Tasks for .NET API Referansı
description: Project yöntem. Tüm proje görevleri kimliklerini anahat düzeylerini başlangıç/bitiş tarihlerini yeniden planlar erken/geç tarihleri ayarlar boşlukları iş ve maliyet alanlarını hesaplar.
type: docs
weight: 1120
url: /tr/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Tüm proje görevleri kimliklerini, anahat düzeylerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/geç tarihleri ayarlar, boşlukları, iş ve maliyet alanlarını hesaplar.

```csharp
public void Recalculate()
```

### Ayrıca bakınız

* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

İsteğe bağlı doğrulama ile tüm proje görevleri kimliklerini, anahat düzeylerini, başlangıç/bitiş tarihlerini yeniden planlar, erken/geç tarihleri ayarlar, boşlukları, iş ve maliyet alanlarını hesaplar.

```csharp
public void Recalculate(bool validate)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| validate | Boolean | Doğruysa, yeniden hesaplama doğrulaması gerçekleştirilecektir. Hangi veriler doğrulanır: Şu anda yalnızca görev ve görev bağlantısı tarih aralıklarının temel doğrulaması uygulanmaktadır. Görevin tarih aralıkları (örn. ActualStart - ActualFinish, EarlyStart - EarlyFinish, vb. ) ve Görev Bağlantıları tarihleri, başlangıç tarihinin bitiş tarihinden küçük veya eşit olduğu tarih kriterlerine göre kontrol edilecektir. Yukarıda açıklanan koşullardan herhangi biri başarısız olursa, o zaman[`RecalculationValidationException`](../../recalculationvalidationexception/)atılacak. |

### Ayrıca bakınız

* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)


