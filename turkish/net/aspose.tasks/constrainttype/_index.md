---
title: Enum ConstraintType
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.ConstraintType Sıralama. Bir görevin başlangıç veya bitiş tarihindeki kısıtlamayı belirtir.
type: docs
weight: 330
url: /tr/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Bir görevin başlangıç veya bitiş tarihindeki kısıtlamayı belirtir.

```csharp
public enum ConstraintType
```

### değerler

| İsim | Değer | Tanım |
| --- | --- | --- |
| Undefined | `-1` | Değer, orijinal proje dosyasında tanımlanmadı. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) Ve[`Finish`](../tsk/finish/) tarihleri[`Task`](../task/) ebeveyne göre ASAP planlanmıştır[`Start`](../tsk/start/) Ve[`Finish`](../tsk/finish/)tarihler ve dikkate alma[`TaskLinks`](../project/tasklinks/) . |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) Ve[`Finish`](../tsk/finish/) tarihleri[`Task`](../task/) ebeveyne göre ALAP planlanmıştır[`Start`](../tsk/start/) Ve[`Finish`](../tsk/finish/)tarihler ve dikkate alma[`TaskLinks`](../project/tasklinks/) . |
| MustStartOn | `2` | , Tarihinde Başlamalı |
| MustFinishOn | `3` | Bitmeli |
| StartNoEarlierThan | `4` | Şu Tarihten Daha Önce Başlatma |
| StartNoLaterThan | `5` | En Geç Başlangıç Tarihi: |
| FinishNoEarlierThan | `6` | Bitiş Tarihi: |
| FinishNoLaterThan | `7` | En Geç Bitecek |

### Notlar

XML'e dışa aktarırken, Tanımsız değerler elde edilen XML'den çıkarılacaktır.

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks/)
* toplantı [Aspose.Tasks](../../)


