---
title: Project.UpdateProjectWorkAsComplete
second_title: Aspose.Tasks for .NET API Referansı
description: Project yöntem. Projenin tamamı için belirtilen bir tarihe kadar tüm işleri eksiksiz olarak günceller.
type: docs
weight: 1250
url: /tr/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

Projenin tamamı için belirtilen bir tarihe kadar tüm işleri eksiksiz olarak günceller.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| completeThrough | DateTime | İşin tamamlandığı şekliyle güncelleneceği tarih. |
| setZeroOrHundredPercentCompleteOnly | Boolean | True olarak ayarlanırsa, yalnızca bitiş tarihi belirtilen tamamlama tarihinden önce olan görevleri %100 tamamlandı olarak günceller. Aksi takdirde, programlanan başlangıç ve tamamlama tarihlerine göre bir tamamlanma yüzdesi değeri hesaplar. |

### Ayrıca bakınız

* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

Güncellemelerin tümü, belirtilen görev listesi için belirtilen tarihe kadar tamamlanmış olarak çalışır.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| completeThrough | DateTime | İşin tamamlandığı şekliyle güncelleneceği tarih. |
| setZeroOrHundredPercentCompleteOnly | Boolean | True olarak ayarlanırsa, yalnızca bitiş tarihi belirtilen tamamlama tarihinden önce olan görevleri %100 tamamlandı olarak günceller. Aksi takdirde, programlanan başlangıç ve tamamlama tarihlerine göre bir tamamlanma yüzdesi değeri hesaplar. |
| taskCollection | List`1 | Çalışmayı güncellemek için görevlerin&lt;Görev&gt; listesi. |

### Ayrıca bakınız

* class [Task](../../task/)
* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)


