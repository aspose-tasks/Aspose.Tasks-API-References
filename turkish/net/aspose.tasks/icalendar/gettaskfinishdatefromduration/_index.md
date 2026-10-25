---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ICalendar yöntemi. Görevin bitiş tarih ve saatini, başlangıç tarihinin bölünmüş parçalarından ve çalışma süresinden hesaplar."
type: docs
weight: 50
url: /tr/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Görevin başlangıç tarihi, bölünmüş parçaları ve çalışma süresinden görev bitiş tarih ve saatini hesaplar.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Bitiş tarihini hesaplamak için görev. |
| süre | TimeSpan | Hesaplanacak süre. |

### Dönüş Değeri

Verilen başlangıç tarihi ve süre için görevin bitiş tarihi.

## Açıklamalar

Görev özet ise, null ise veya başlangıç tarihi ayarlanmamışsa DateTime.MinValue döndürür.

### Ayrıca Bakınız

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


