---
title: UpdateProjectWorkAsComplete
second_title: Aspose.Tasks for .NET API Referansı
description: Tüm çalışmaları tüm proje için belirtilen bir tarihe kadar eksiksiz olarak günceller.
type: docs
weight: 470
url: /tr/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

Tüm çalışmaları, tüm proje için belirtilen bir tarihe kadar eksiksiz olarak günceller.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| completeThrough | DateTime | İşin tamamlandığı şekliyle güncelleneceği tarih. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Doğru olarak ayarlanırsa, yalnızca bitiş tarihi belirtilen tamamlama tarihinden önce olan %100 tamamlandı olarak bu görevleri günceller. Aksi takdirde, planlanan başlangıç ve tamamlama tarihlerine göre bir tamamlanma yüzdesi değeri hesaplar. |

### Ayrıca bakınız

* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

Belirtilen görev listesi için belirtilen bir tarihe kadar tüm çalışmaları eksiksiz olarak günceller.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| completeThrough | DateTime | İşin tamamlandığı şekliyle güncelleneceği tarih. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Doğru olarak ayarlanırsa, yalnızca bitiş tarihi belirtilen tamamlama tarihinden önce olan %100 tamamlandı olarak bu görevleri günceller. Aksi takdirde, planlanan başlangıç ve tamamlama tarihlerine göre bir tamamlanma yüzdesi değeri hesaplar. |
| taskCollection | List`1 | Çalışmanın güncelleştirileceği görevlerin &lt;Görev&gt; listesi. |

### Ayrıca bakınız

* class [Task](../../task)
* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->