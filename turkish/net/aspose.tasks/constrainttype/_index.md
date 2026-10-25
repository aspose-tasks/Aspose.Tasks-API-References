---
title: "Enum ConstraintType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ConstraintType enum. Bir görevin başlangıç veya bitiş tarihine uygulanan kısıtlamayı belirtir"
type: docs
weight: 330
url: /tr/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Bir görevin başlangıç veya bitiş tarihine ilişkin kısıtlamayı belirtir.

```csharp
public enum ConstraintType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Değer, orijinal proje dosyasında tanımlanmamıştı. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) ve [`Finish`](../tsk/finish/) tarihleri, ebeveyn [`Start`](../tsk/start/) ve [`Finish`](../tsk/finish/) tarihleri dikkate alınarak ve [`TaskLinks`](../project/tasklinks/) göz önüne alınarak mümkün olan en kısa sürede planlanır. |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) ve [`Finish`](../tsk/finish/) tarihleri [`Task`](../task/) üst [`Start`](../tsk/start/) ve [`Finish`](../tsk/finish/) tarihlerine göre ALAP olarak planlanır ve [`TaskLinks`](../project/tasklinks/) dikkate alınır. |
| MustStartOn | `2` | Başlaması Gereken |
| MustFinishOn | `3` | Bitişi Gereken |
| StartNoEarlierThan | `4` | Başlangıç En Erken |
| StartNoLaterThan | `5` | Başlangıç En Geç |
| FinishNoEarlierThan | `6` | Bitiş En Erken |
| FinishNoLaterThan | `7` | Bitiş En Geç |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Görev için ConstraintType.AsSoonAsPossible kısıtlamasını nasıl ayarlayacağınızı gösterir &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt;.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Id 11 olan görev için As Soon As Possible kısıtlamasını ayarla.
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


