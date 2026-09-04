---
title: "Aspose::Tasks::Project::Recalculate metodu"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "C++ için Aspose.Tasks"
description: "Tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden zamanlar, erken/geç tarihlerini ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar."
type: docs
weight: 1130
url: /tr/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

Tüm proje görevlerinin kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden zamanlar, erken/geç tarihlerini ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

Tüm proje görev kimliklerini, taslak seviyelerini, başlangıç/bitiş tarihlerini yeniden zamanlar, erken/geç tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını isteğe bağlı doğrulama ile hesaplar.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| Parametre | Açıklama |
| --- | --- |
| doğrula | Doğru ise yeniden hesaplamanın doğrulaması gerçekleştirilecektir. Hangi verilerin doğrulandığı: Şu anda yalnızca görev ve görev bağlantısı tarih aralıklarının temel doğrulaması uygulanmaktadır. Görevlerin tarih aralıkları (ör. ActualStart - ActualFinish, EarlyStart - EarlyFinish, vb.) ve Görev Bağlantıları tarihleri, başlangıç tarihinin bitiş tarihine eşit veya daha küçük olduğu tarih kriterine göre kontrol edilecektir. Yukarıda açıklanan koşullardan herhangi biri başarısız olursa RecalculationValidationException istisnası fırlatılacaktır. |

