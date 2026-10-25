---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete metodu"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "C++ için Aspose.Tasks"
description: "Belirtilen tarih itibarıyla tüm işi tamamlanmış olarak günceller ve tüm proje için."
type: docs
weight: 2080
url: /tr/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Belirtilen tarih itibarıyla tüm işi tamamlanmış olarak günceller ve tüm proje için.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Parametre | Açıklama |
| --- | --- |
| completeThrough | Tamamlanmış olarak çalışmayı güncellemek için tarih. |
| setZeroOrHundredPercentCompleteOnly | Eğer true olarak ayarlanırsa, belirtilen tamamlanma tarihinden önce bitiş tarihine sahip görevleri %100 tamamlanmış olarak günceller. Aksi takdirde, planlanan başlangıç ve tamamlanma tarihine göre bir yüzde tamamlanma değeri hesaplar. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Belirtilen görev listesi için belirli bir tarihe kadar tüm çalışmayı tamamlanmış olarak günceller.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Parametre | Açıklama |
| --- | --- |
| completeThrough | Tamamlanmış olarak çalışmayı güncellemek için tarih. |
| setZeroOrHundredPercentCompleteOnly | Eğer true olarak ayarlanırsa, belirtilen tamamlanma tarihinden önce bitiş tarihine sahip görevleri %100 tamamlanmış olarak günceller. Aksi takdirde, planlanan başlangıç ve tamamlanma tarihine göre bir yüzde tamamlanma değeri hesaplar. |
| taskCollection | Çalışmanın güncelleneceği görevlerin List< Task >. |

