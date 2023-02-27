---
title: Class CsvOptions
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.Saving.CsvOptions sınıf. Projeyi CSVye kaydederken ek seçenekler belirlemeye izin verir.
type: docs
weight: 1720
url: /tr/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Projeyi CSV'ye kaydederken ek seçenekler belirlemeye izin verir.

```csharp
public class CsvOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [CsvOptions](csvoptions/)() | Yeni bir örneğini başlatır.`CsvOptions` projeyi CSV biçiminde kaydetmek için kullanılabilecek sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Örneklerin listesini alır veya ayarlar.[`BarStyle`](../../aspose.tasks.visualization/barstyle/) proje görünümünde görünen sınıf. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Nokta cinsinden özel sayfa boyutunu alır veya ayarlar (1 punto = 1/72 inç). |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Kaydedilecek bir veri kategorisi alır veya ayarlar. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Çalışma dışı zamanın çekilip çekilmeyeceğini gösteren bir değer alır veya ayarlar (Varsayılan değer DOĞRU'dur). |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | CSV'yi. ile kaydetmek için bir kodlama alır veya ayarlar |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | İşlemeyi bitirmek için bir tarih alır veya ayarlar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Satır yüksekliğinin içeriğine sığması için artırılıp artırılmayacağını belirten bir değer alır veya ayarlar. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Bir görünümün takvim bölümünün son sayfanın sonuna (sağ tarafa) işlenmesi gerekip gerekmediğini alır veya ayarlar. Değer yanlışsa, sayfada boş bir alan olsa bile takvim bölümü tam olarak EndDate'e dönüştürülür. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Bir liste alır veya ayarlar[`Gridline`](../../aspose.tasks.visualization/gridline/) proje görünümünde görünen. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Başlıkların dahil edilip edilmeyeceğini gösteren bir değer alır veya ayarlar (varsayılan değer TRUE'dur). |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Açıklamanın her sayfada gösterilip gösterilmeyeceğini gösteren bir değer alır veya ayarlar (Varsayılan değer DOĞRU'dur). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Kritik görevlerin kırmızı renkte görüntülenip görüntülenmeyeceğini belirten bir değer alır veya ayarlar (Varsayılan değer FALSE'dir). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Çalışma dışı zaman rengini alır veya ayarlar. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Projenin sayfa sayısını alır veya ayarlar. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | İşlenecek sayfanın boyutunu alır veya ayarlar (Varsayılan değer, PageSize.A4'tür). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Şunu alır veya ayarlar:[`PresentationFormat`](../saveoptions/presentationformat/) belgenin kaydedileceği yer. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Proje grafik biçiminde kaydedildiğinde, bir projenin tek bir sayfaya dönüştürülüp dönüştürülmeyeceğini belirten bir değer alır veya ayarlar . İşlenen projenin bir sayfaya sığabilmesi için sayfa boyutu değiştirilecektir. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini gösteren bir değer alır veya ayarlar. Alt görevler için Toplama alanı, alt görev Gantt çubuklarıyla ilgili bilgilerin özet görev çubuğuna toplanıp toplanmayacağını belirtir. Özet görevler için Toplama alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Herhangi bir alt görevin özetlenmesi için Özet görevler için Toplama alanının Evet olarak ayarlanmış olması gerekir. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | İşlemenin başlayacağı tarihi alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Gantt grafiği ve Görev Sayfası grafiğindeki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı çizelgelerinde işlenen görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Bir metin sınırlayıcı alır veya ayarlar. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Örneklerin listesini alır veya ayarlar.[`TextStyle`](../../aspose.tasks.visualization/textstyle/) proje görünümünde görünen sınıf. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Şunu alır veya ayarlar:[`Timescale`](../saveoptions/timescale/) proje grafik biçiminde kaydedildiğinde zaman ölçeğinin (varsa) nasıl işlendiğini kontrol etmek için kullanılan değer. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Gantt Chart. oluşturulurken degrade fırçasının kullanılması gerekip gerekmediğini belirten bir değer alır veya ayarlar. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | İşlenecek görünüm sütunlarının bir listesini alır veya ayarlar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Ayarlanmazsa görev kimlikleri, görev adları, başlangıç ve bitiş yalnızca işlenir. Hem Görünüm hem de[`ViewSettings`](../saveoptions/viewsettings/)özellikler ayarlandığında, Görünüm'deki sütunlar, ViewSettings. 'deki sütunları geçersiz kılar |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Bir görünüm alır veya ayarlar ([`View`](../saveoptions/view/) ) işlemek için. Hangi görünümün PDF, HTML veya Resim formatlarına kaydedileceğini açıkça belirtmek için bu seçenekleri kullanabilirsiniz. Bu özellik ayarlanırsa,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) proje kaydedildiğinde özellik göz ardı edilir. Görünüm aşağıdaki ekranlardan birinden olmalıdır (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Ayrıca bakınız

* class [SaveOptions](../saveoptions/)
* ad alanı [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* toplantı [Aspose.Tasks](../../)


