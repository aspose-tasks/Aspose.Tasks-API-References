---
title: "ProjectDisplayOptions.ShowTaskScheduleWarnings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectDisplayOptions özelliği. Project, manuel olarak planlanmış bir görevde olası bir zamanlama çakışması tespit ettiğinde uyarı gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Bu seçenek Project 2010 ve sonraki sürümler için kullanılabilir."
type: docs
weight: 90
url: /tr/net/aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/
---
## ProjectDisplayOptions.ShowTaskScheduleWarnings property

Project, manuel olarak planlanmış bir görevde olası bir zamanlama çakışması tespit ettiğinde uyarı gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Bu seçenek Project 2010 sürümü ve sonrasında mevcuttur.

```csharp
public bool ShowTaskScheduleWarnings { get; set; }
```

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

* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


