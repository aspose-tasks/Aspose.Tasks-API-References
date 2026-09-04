---
title: "Aspose::Tasks::Task::MoveToSibling metodu"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "C++ için Aspose.Tasks"
description: "Mevcut görevi aynı Taslak Düzeyinde belirtilen görevin önüne taşır."
type: docs
weight: 1370
url: /tr/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Mevcut görevi aynı Outline Level'da belirtilen görevin önüne taşır. ParentProject.CalculationMode None ise, bu yöntemi kullandıktan sonra kullanıcı Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihlerini, erken/son tarihleri ayarlar) yeniden zamanlar ve gecikmeler, iş ve maliyet alanları, outline seviyeleri gibi bağımlı alanları hesaplar). ParentProject.CalculationMode Manual ise yöntem yalnızca görev kimliğini, outline seviyesini ve outline numaralarını otomatik olarak hesaplar. ParentProject.CalculationMode Automatic ise yöntem tüm projenin görevlerini otomatik olarak yeniden zamanlar (başlangıç/bitiş tarihlerini, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, kimlikleri ve outline seviyelerini yeniden hesaplar).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Parametre | Açıklama |
| --- | --- |
| beforeTask | Mevcut görevin ekleneceği görev. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Mevcut görevi aynı Taslak Düzeyinde belirtilen Id'ye sahip bir görevin önüne taşır. Eğer ParentProject.CalculationMode None ise, kullanıcı bu metodu kullandıktan sonra Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihlerini, erken/geç tarihlerini ayarlar) yeniden zamanlayacak ve gecikmeler, iş ve maliyet alanları, taslak düzeyleri gibi bağımlı alanları hesaplayacaktır). Eğer ParentProject.CalculationMode Manual ise, metod yalnızca görev id'sini, taslak düzeyini ve taslak numaralarını otomatik olarak hesaplayacaktır. Eğer ParentProject.CalculationMode Automatic ise, metod tüm projenin görevlerini otomatik olarak yeniden zamanlayacaktır (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, id'leri ve taslak düzeylerini yeniden hesaplar).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Parametre | Açıklama |
| --- | --- |
| beforeTaskId | Mevcut görevin ekleneceği görevin Id'si ( Tsk::Id ). |

