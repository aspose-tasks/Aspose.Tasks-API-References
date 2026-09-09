---
title: "Sınıf UsageView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.UsageView sınıfı. Bir projedeki kullanım görünümünü temsil eder"
type: docs
weight: 2650
url: /tr/net/aspose.tasks/usageview/
---
## UsageView class

Bir projede kullanım görünümünü temsil eder.

```csharp
public abstract class UsageView : View
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Ayrıntı veri hizalamasını alır veya ayarlar. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Görünümün alt zaman ölçeği katmanının ayarlarını alır veya ayarlar. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Görünümde ayrıntı başlık sütununun gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Kısa detay başlık adlarının görüntülenip görüntülenmeyeceğini belirten bir değeri alır veya ayarlar. |
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

Görev kullanım görünümünü detaylarla nasıl render edeceğini gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// görünümü al
UsageView view = (TaskUsageView)project.DefaultView;

// detay başlık sütunu görüntülenmeyecek
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// detay başlık sütununu görüntüle
view.DisplayDetailsHeaderColumn = true;

// tüm atama satırlarında detay başlığını tekrarla
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Ayrıca Bakınız

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


