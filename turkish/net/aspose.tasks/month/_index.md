---
title: "Enum Month"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Month enum. Ayı belirtir."
type: docs
weight: 1040
url: /tr/net/aspose.tasks/month/
---
## Month enumeration

Ayı belirtir.

```csharp
public enum Month
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Değerin orijinal proje dosyasında tanımlanmadığını gösterir. |
| January | `0` | Ocak ayını gösterir. |
| February | `1` | Şubat ayını gösterir. |
| March | `2` | Mart ayını gösterir. |
| April | `3` | Nisan ayını gösterir. |
| May | `4` | Mayıs ayını gösterir. |
| June | `5` | Haziran ayını gösterir. |
| July | `6` | Temmuz ayını gösterir. |
| August | `7` | Ağustos ayını gösterir. |
| September | `8` | Eylül ayını gösterir. |
| October | `9` | Ekim ayını gösterir. |
| November | `10` | Kasım ayını gösterir. |
| December | `11` | Aralık ayını gösterir. |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Yeni yinelenen görevler oluştururken yıl günü tekrarlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


