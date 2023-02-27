---
title: Class ImageSaveOptions
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.Saving.ImageSaveOptions sınıf. Proje sayfalarını görüntülere dönüştürürken ek seçenekler belirlemeye izin verir.
type: docs
weight: 1770
url: /tr/net/aspose.tasks.saving/imagesaveoptions/
---
## ImageSaveOptions class

Proje sayfalarını görüntülere dönüştürürken ek seçenekler belirlemeye izin verir.

```csharp
public class ImageSaveOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFileFormat) | Yeni bir örneğini başlatır.`ImageSaveOptions` işlenmiş görüntüleri TIFF, PNG, BMP veya JPEG formatlarında kaydetmek için kullanılabilen sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Örneklerin listesini alır veya ayarlar.[`BarStyle`](../../aspose.tasks.visualization/barstyle/) proje görünümünde görünen sınıf. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Nokta cinsinden özel sayfa boyutunu alır veya ayarlar (1 punto = 1/72 inç). |
| [DefaultFontName](../../aspose.tasks.saving/imagesaveoptions/defaultfontname/) { get; set; } | Oluşturma için varsayılan yazı tipini alır veya ayarlar. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Çalışma dışı zamanın çekilip çekilmeyeceğini gösteren bir değer alır veya ayarlar (Varsayılan değer DOĞRU'dur). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | İşlemeyi bitirmek için bir tarih alır veya ayarlar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Satır yüksekliğinin içeriğine sığması için artırılıp artırılmayacağını belirten bir değer alır veya ayarlar. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Bir görünümün takvim bölümünün son sayfanın sonuna (sağ tarafa) işlenmesi gerekip gerekmediğini alır veya ayarlar. Değer yanlışsa, sayfada boş bir alan olsa bile takvim bölümü tam olarak EndDate'e dönüştürülür. |
| [FontResolveCallback](../../aspose.tasks.saving/imagesaveoptions/fontresolvecallback/) { get; set; } | Çözülmüş yazı tiplerini özelleştirmek için kullanılabilecek bir geri arama alır veya ayarlar. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Bir liste alır veya ayarlar[`Gridline`](../../aspose.tasks.visualization/gridline/) proje görünümünde görünen. |
| [HorizontalResolution](../../aspose.tasks.saving/imagesaveoptions/horizontalresolution/) { get; set; } | dpi. 'de yatay çözünürlüğü alır veya ayarlar |
| [JpegQuality](../../aspose.tasks.saving/imagesaveoptions/jpegquality/) { get; set; } | Bir JPEG kalitesi alır veya ayarlar. İzin verilen değer aralığı 0..100. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Açıklamanın her sayfada gösterilip gösterilmeyeceğini gösteren bir değer alır veya ayarlar (Varsayılan değer DOĞRU'dur). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Kritik görevlerin kırmızı renkte görüntülenip görüntülenmeyeceğini belirten bir değer alır veya ayarlar (Varsayılan değer FALSE'dir). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Çalışma dışı zaman rengini alır veya ayarlar. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Projenin sayfa sayısını alır veya ayarlar. |
| [Pages](../../aspose.tasks.saving/imagesaveoptions/pages/) { get; set; } | Proje düzenini ayrı dosyalara kaydederken kaydedilecek sayfa numaralarının bir listesini alır veya ayarlar. Bu liste boşsa tüm sayfalar kaydedilecektir. |
| [PageSavingCallback](../../aspose.tasks.saving/imagesaveoptions/pagesavingcallback/) { get; set; } | Oluşturulan her sayfa için bir çıktı akışı almak için kullanılan, kullanıcı tanımlı bir geri çağırma alır veya ayarlar. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | İşlenecek sayfanın boyutunu alır veya ayarlar (Varsayılan değer, PageSize.A4'tür). |
| [PixelFormat](../../aspose.tasks.saving/imagesaveoptions/pixelformat/) { get; set; } | Görüntüdeki her piksel için renk verilerinin biçimini alır veya ayarlar. |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Şunu alır veya ayarlar:[`PresentationFormat`](../saveoptions/presentationformat/) belgenin kaydedileceği yer. |
| [ReduceFooterGap](../../aspose.tasks.saving/imagesaveoptions/reducefootergap/) { get; set; } | Son görev ile altbilgi arasındaki boşluğun azaltılması gerekip gerekmediğini gösteren bir değer alır veya ayarlar. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Proje grafik biçiminde kaydedildiğinde, bir projenin tek bir sayfaya dönüştürülüp dönüştürülmeyeceğini belirten bir değer alır veya ayarlar . İşlenen projenin bir sayfaya sığabilmesi için sayfa boyutu değiştirilecektir. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini gösteren bir değer alır veya ayarlar. Alt görevler için Toplama alanı, alt görev Gantt çubuklarıyla ilgili bilgilerin özet görev çubuğuna toplanıp toplanmayacağını belirtir. Özet görevler için Toplama alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Herhangi bir alt görevin özetlenmesi için Özet görevler için Toplama alanının Evet olarak ayarlanmış olması gerekir. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | İşlemenin başlayacağı tarihi alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Gantt grafiği ve Görev Sayfası grafiğindeki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı çizelgelerinde işlenen görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Örneklerin listesini alır veya ayarlar.[`TextStyle`](../../aspose.tasks.visualization/textstyle/) proje görünümünde görünen sınıf. |
| [TiffCompression](../../aspose.tasks.saving/imagesaveoptions/tiffcompression/) { get; set; } | Oluşturulan görüntüleri TIFF biçiminde kaydederken uygulanacak sıkıştırma türünü alır veya ayarlar. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Şunu alır veya ayarlar:[`Timescale`](../saveoptions/timescale/) proje grafik biçiminde kaydedildiğinde zaman ölçeğinin (varsa) nasıl işlendiğini kontrol etmek için kullanılan değer. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Gantt Chart. oluşturulurken degrade fırçasının kullanılması gerekip gerekmediğini belirten bir değer alır veya ayarlar. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/) { get; set; } | Oluşturma için varsayılan yazı tipinin kullanılması gerekip gerekmediğini belirten bir değer alır veya ayarlar. |
| [VerticalResolution](../../aspose.tasks.saving/imagesaveoptions/verticalresolution/) { get; set; } | dpi. 'de dikey çözünürlüğü alır veya ayarlar |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | İşlenecek görünüm sütunlarının bir listesini alır veya ayarlar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Ayarlanmazsa görev kimlikleri, görev adları, başlangıç ve bitiş yalnızca işlenir. Hem Görünüm hem de[`ViewSettings`](../saveoptions/viewsettings/)özellikler ayarlandığında, Görünüm'deki sütunlar, ViewSettings. 'deki sütunları geçersiz kılar |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Bir görünüm alır veya ayarlar ([`View`](../saveoptions/view/) ) işlemek için. Hangi görünümün PDF, HTML veya Resim formatlarına kaydedileceğini açıkça belirtmek için bu seçenekleri kullanabilirsiniz. Bu özellik ayarlanırsa,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) proje kaydedildiğinde özellik göz ardı edilir. Görünüm aşağıdaki ekranlardan birinden olmalıdır (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Ayrıca bakınız

* class [SaveOptions](../saveoptions/)
* ad alanı [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* toplantı [Aspose.Tasks](../../)


