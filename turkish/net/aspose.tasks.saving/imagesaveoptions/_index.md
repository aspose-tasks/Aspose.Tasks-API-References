---
title: "Sınıf ImageSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.ImageSaveOptions sınıfı. Proje sayfalarını görüntülere render ederken ek seçenekler belirtmeye olanak tanır"
type: docs
weight: 2030
url: /tr/net/aspose.tasks.saving/imagesaveoptions/
---
## ImageSaveOptions class

Proje sayfalarını görüntülere render ederken ek seçenekleri belirtmeye izin verir.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFileFormat) | `ImageSaveOptions` sınıfının, render edilen görüntüleri TIFF, PNG, BMP veya JPEG formatlarında kaydetmek için kullanılabilecek yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Proje görünümünde görünen [`BarStyle`](../../aspose.tasks.visualization/barstyle/) sınıfının örneklerinin listesini alır veya ayarlar. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Özel sayfa boyutunu nokta cinsinden alır veya ayarlar (1 nokta = inçin 1/72'si). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değeri alır veya ayarlar (Varsayılan değer TRUE'dır). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Render işleminin tamamlanacağı tarihi alır veya ayarlar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Satır yüksekliğinin içeriğe sığacak şekilde artırılıp artırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [FontSettings](../../aspose.tasks.saving/imagesaveoptions/fontsettings/) { get; } | Projenin görünümü render edilirken kullanılan yazı tipi ayarlarını belirtir. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Proje görünümünde görünen bir [`Gridline`](../../aspose.tasks.visualization/gridline/) listesini alır veya ayarlar. |
| [HorizontalResolution](../../aspose.tasks.saving/imagesaveoptions/horizontalresolution/) { get; set; } | Yatay çözünürlüğü dpi cinsinden alır veya ayarlar. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Sayfa yönünün dikey olup olmadığını gösteren bir değeri alır veya ayarlar; sayfa yönü yataysa false döndürür. |
| [JpegQuality](../../aspose.tasks.saving/imagesaveoptions/jpegquality/) { get; set; } | JPEG kalitesini alır veya ayarlar. İzin verilen değer aralığı 0..100'dür. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Bir lejantın nasıl render edileceğini tanımlayan bir değeri alır veya ayarlar. Varsayılan değer LegendDrawingOptions.OnEveryPage'dir. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Sayfa lejantında hangi çubukların render edileceğini tanımlayan bir PageLegendItem dizisini alır veya ayarlar. Null ise, varsayılan öğeler render edilir. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar (Varsayılan değer FALSE'tır). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Çalışma dışı zaman rengini alır veya ayarlar. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Projenin sayfa sayısını alır veya ayarlar. |
| [Pages](../../aspose.tasks.saving/imagesaveoptions/pages/) { get; set; } | Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesini alır veya ayarlar. Liste boşsa tüm sayfalar kaydedilir. |
| [PageSavingCallback](../../aspose.tasks.saving/imagesaveoptions/pagesavingcallback/) { get; set; } | Her render edilen sayfa için bir çıktı akışı almakta kullanılan kullanıcı tanımlı geri çağırmayı alır veya ayarlar. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Render edilecek sayfanın boyutunu alır veya ayarlar (Varsayılan değer PageSize.A4'tür). |
| [PixelFormat](../../aspose.tasks.saving/imagesaveoptions/pixelformat/) { get; set; } | Görüntüdeki her piksel için renk verisinin formatını alır veya ayarlar. |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Belgenin kaydedileceği [`PresentationFormat`](../saveoptions/presentationformat/) değerini alır veya ayarlar. |
| [ReduceFooterGap](../../aspose.tasks.saving/imagesaveoptions/reducefootergap/) { get; set; } | Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri alır veya ayarlar. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Proje grafik formatında kaydedildiğinde tek bir sayfaya render edilip edilmeyeceğini gösteren bir değeri alır veya ayarlar. Sayfa boyutu, render edilen projenin tek bir sayfaya sığacak şekilde değiştirilecektir. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini gösteren bir değeri alır veya ayarlar. Alt görevler için Rollup alanı, alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını gösterir. Özet görevler için Rollup alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Alt görevlere toplanabilmesi için özet görevlerin Rollup alanının Evet olarak ayarlanmış olması gerekir. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Renderlamaya başlanacak tarihi alır veya ayarlar. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Görev bağlantılarının renderlanmasının bazı yönlerini özelleştirmek için kullanılabilecek bir geri çağırma işlevini alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı şemalarında renderlanan görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Bir proje görünümünün renderlanması sırasında uygulanan metin stillerinin listesini alır veya ayarlar. |
| [TiffCompression](../../aspose.tasks.saving/imagesaveoptions/tiffcompression/) { get; set; } | Oluşturulan görüntüleri TIFF formatında kaydederken uygulanacak sıkıştırma türünü alır veya ayarlar. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Proje grafik formatında kaydedildiğinde zaman ölçeğinin (varsa) nasıl renderlanacağını kontrol etmek için kullanılan [`Timescale`](../saveoptions/timescale/) değerini alır veya ayarlar. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Zaman ölçeğinin sağ ucunun sayfa sonu ile nasıl hizalanacağını tanımlayan davranışı alır veya ayarlar. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Gantt Şeması render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirten bir değeri alır veya ayarlar. |
| [VerticalResolution](../../aspose.tasks.saving/imagesaveoptions/verticalresolution/) { get; set; } | Dikey çözünürlüğü dpi cinsinden alır veya ayarlar. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Renderlanacak görünüm sütunlarının listesini alır veya ayarlar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Ayarlanmamışsa yalnızca görev kimlikleri, görev adları, başlangıç ve bitiş renderlanır. Hem View hem de [`ViewSettings`](../saveoptions/viewsettings/) özellikleri ayarlanmışsa, View'tan gelen sütunlar ViewSettings'ten gelen sütunların üzerine yazar. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Renderlanacak bir görünümü ([`View`](../saveoptions/view/)) alır veya ayarlar. Bu seçeneği, hangi görünümün PDF, HTML veya Görüntü formatlarında kaydedileceğini açıkça belirtmek için kullanabilirsiniz. Bu özellik ayarlanırsa, proje kaydedildiğinde [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) özelliği göz ardı edilir. Görünüm, aşağıdaki ekranlardan biri olmalıdır (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

## Örnekler

Projeyi bir akışa görüntü olarak nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // ImageSaveOptions kullanarak projeyi görüntü formatında kaydederiz
    project.Save(stream, options);
}
```

### Ayrıca Bakınız

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


