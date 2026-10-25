---
title: "Sınıf TaskUsageView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskUsageView sınıfı. Bir projedeki görev kullanım görünümünü temsil eder"
type: docs
weight: 2480
url: /tr/net/aspose.tasks/taskusageview/
---
## TaskUsageView class

Bir projedeki görev kullanım görünümünü temsil eder.

```csharp
public class TaskUsageView : UsageView
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Ayrıntı veri hizalamasını alır veya ayarlar. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Görünümün alt zaman ölçeği katmanının ayarlarını alır veya ayarlar. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Görünümde ayrıntı başlık sütununun gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Kısa detay başlık adlarının görüntülenip görüntülenmeyeceğini belirten bir değeri alır veya ayarlar. |
| [FieldCollection](../../aspose.tasks/taskusageview/fieldcollection/) { get; } | Bu TaskUsageView'in [`TaskUsageViewFieldCollection`](../taskusageviewfieldcollection/) nesnesini alır. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Tek bir görünümde kullanılan bir filtreyi alır veya ayarlar. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Tek bir görünümün grubunu alır veya ayarlar. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamayacağını belirten bir değeri alır veya ayarlar. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Görünümün orta zaman ölçeği katmanının ayarlarını alır veya ayarlar. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Bir View nesnesinin adını alır veya ayarlar. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | [`PageInfo`](../view/pageinfo/) sınıfının bir örneğini alır. mpp dosya formatında bulunan sayfa ayarı verilerini temsil eder. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View nesnesinin üst nesnesini alır. Salt okunur [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Tüm atama satırlarında detay başlığının tekrarlanıp tekrarlanmayacağını belirten bir değeri alır veya ayarlar. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Tek bir görünüm için ekran tipini alır. Salt okunur [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project'in tek bir görünüm adını Şerit'teki Görünüm veya Diğer Görünümler açılır listelerinde gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Tek bir görünümün tablosunu alır veya ayarlar. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Görünümün üst zaman ölçeği katmanının ayarlarını alır veya ayarlar. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | Tek bir görünümdeki öğenin türünü alır, örneğin görevler veya kaynaklar. Salt okunur [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Bir görünümün benzersiz tanımlayıcısını alır. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Görünümdeki [`OleObject`](../oleobject/) yerleşimini ve görünümünü temsil eden nesneler koleksiyonunu alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Mevcut örneği aynı türdeki başka bir nesneyle karşılaştırır ve mevcut örneğin diğer nesneye göre sıralama düzeninde önce mi, sonra mı yoksa aynı konumda mı olduğunu belirten bir tam sayı döndürür. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | [`Resource`](../resource/) sınıfının örneği için bir karma kod değeri döndürür. |

## Örnekler

Görünüm ayarlarında tanımlanan zaman ölçeği ayarlarıyla görev kullanım görünümünün nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// SaveOptions'ı tanımlayın ve TaskUsageView zaman ölçeği ayarlarının kullanılmasını belirtin.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

Önceden tanımlı zaman ölçeği ayarlarıyla görev kullanım görünümünün nasıl render edileceğini gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

// SaveOptions'ı tanımlayın ve önceden tanımlı TimeScale ayarları 'Days'ı belirtin.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Days,

    // Presentation formatını TaskUsage olarak ayarlayın
    PresentationFormat = PresentationFormat.TaskUsage
};

var outputProject = "TaskUsageView_result_days_out.pdf";
project.Save(OutDir + outputProject, options);

// Timescale ayarlarını ThirdsOfMonths olarak ayarlayın
options.Timescale = Timescale.ThirdsOfMonths;

outputProject = "TaskUsageView_result_thirdsOfMonths_out.pdf";
project.Save(OutDir + outputProject, options);

// Timescale ayarlarını Months olarak ayarlayın
options.Timescale = Timescale.Months;

outputProject = "TaskUsageView_result_months_out.pdf";
project.Save(OutDir + outputProject, options);
```

### Ayrıca Bakınız

* class [UsageView](../usageview/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


