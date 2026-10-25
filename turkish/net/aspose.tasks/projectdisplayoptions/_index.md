---
title: "Sınıf ProjectDisplayOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ProjectDisplayOptions sınıfı. Bir proje örneği için görüntüleme seçeneklerini temsil eder."
type: docs
weight: 1450
url: /tr/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Bir proje örneği için görüntüleme seçeneklerini temsil eder.

```csharp
public class ProjectDisplayOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | `ProjectDisplayOptions` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Sayı değeri ve zaman kısaltması (1 wk yerine 1wk) önüne boşluk eklenip eklenmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Gün etiketinin nasıl görüntüleneceğini alır veya ayarlar. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Saat etiketinin nasıl görüntüleneceğini alır veya ayarlar. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Dakika etiketinin nasıl görüntüleneceğini alır veya ayarlar. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Ay etiketinin nasıl görüntüleneceğini alır veya ayarlar. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Gantt Şeması görünümünün üst kısmında kendi özet görev çubuğuna sahip tek bir satırda tüm proje hakkında özet bilgilerin görüntülenip görüntülenmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Project, manuel planlanmış bir görevle olası bir zamanlama çakışması tespit ettiğinde önerilerin gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Bu seçenek Project 2010 ve sonraki sürümler için mevcuttur. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Project, manuel olarak planlanmış bir görevde olası bir zamanlama çakışması tespit ettiğinde uyarı gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Bu seçenek Project 2010 sürümü ve sonrasında mevcuttur. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Köprülerin altını çizip çizilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Hafta etiketinin nasıl görüntüleneceğini alır veya ayarlar. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Yıl etiketinin nasıl görüntüleneceğini alır veya ayarlar. |

## Örnekler

Projenin görüntüleme seçeneklerinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Project, manuel olarak planlanmış bir görevde olası bir zamanlama çakışması tespit ettiğinde uyarı gösterilip gösterilmeyeceğini belirten bir değeri ayarlar.
// Bu seçenek Project 2010 sürümü ve sonrasında kullanılabilir.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// Sayı değeri ve zaman kısaltması (1 wk yerine 1wk) arasına boşluk eklenip eklenmeyeceğini belirten bir değer
project.DisplayOptions.AddSpaceBeforeLabel = true;

// dakika etiketinin nasıl görüntüleneceğini ayarlar
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// saat etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// Gün etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// Hafta etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// ay etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// yıl etiketinin nasıl görüntüleneceğini ayarla
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// Gantt Chart görünümünün üst kısmında kendi özet görev çubuğu ile tüm proje hakkında özet bilgilerin tek bir satırda gösterilip gösterilmeyeceğini belirten bir değeri ayarla.
project.DisplayOptions.ShowProjectSummaryTask = true;

// Project, manuel olarak planlanmış bir görevde olası bir zamanlama çakışması tespit ettiğinde önerilerin gösterilip gösterilmeyeceğini belirten bir değeri ayarla.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// Köprülerin altının çizilip çizilmeyeceğini belirten bir değeri ayarla.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


