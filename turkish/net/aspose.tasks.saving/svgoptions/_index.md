---
title: SvgOptions
second_title: Aspose.Tasks for .NET API Referansı
description: Proje sayfalarını SVGye işlerken ek seçenekleri belirlemeye izin verir.
type: docs
weight: 1940
url: /tr/net/aspose.tasks.saving/svgoptions/
---
## SvgOptions class

Proje sayfalarını SVG'ye işlerken ek seçenekleri belirlemeye izin verir.

```csharp
public class SvgOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [SvgOptions](svgoptions)() | Yeni bir örneğini başlatır[`SvgOptions`](../svgoptions) projeyi SVG formatında kaydetmek için kullanılabilecek sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Örneklerin listesini alır veya ayarlar.[`BarStyle`](../../aspose.tasks.visualization/barstyle) proje görünümünde görünen sınıf. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Özel sayfa boyutunu punto cinsinden alır veya ayarlar (1 nokta = 1/72 inç). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Çalışma dışı zamanın çizilmesi gerekip gerekmediğini belirten bir değer alır veya ayarlar (Varsayılan değer DOĞRU'dur). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Oluşturmayı bitirmek için bir tarih alır veya ayarlar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Satır yüksekliğinin içeriğine uyacak şekilde artırılması gerekip gerekmediğini belirten bir değer alır veya ayarlar. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Bir liste alır veya ayarlar[`Gridline`](../../aspose.tasks.visualization/gridline) proje görünümünde görünen. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Göstergenin her sayfada gösterilip gösterilmeyeceğini belirten bir değer alır veya ayarlar (Varsayılan değer DOĞRU'dur). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Kritik görevlerin kırmızı renkte görüntülenip görüntülenmeyeceğini belirten bir değer alır veya ayarlar (Varsayılan değer YANLIŞ'tır). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Çalışmayan zaman rengini alır veya ayarlar. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Projenin sayfa sayısını alır veya ayarlar. |
| [PageSavingCallback](../../aspose.tasks.saving/svgoptions/pagesavingcallback) { get; set; } | Oluşturulan her sayfa için bir çıktı akışı almak için kullanılan kullanıcı tanımlı bir uygulama geri aramasını alır veya ayarlar. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | İşlenecek sayfanın boyutunu alır veya ayarlar (Varsayılan değer PageSize.A4'tür). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Alır veya ayarlar[`PresentationFormat`](../saveoptions/presentationformat) belgenin kaydedileceği yer. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Proje grafik biçiminde kaydedildiğinde, projenin tek bir sayfaya dönüştürülüp dönüştürülmeyeceğini belirten bir değer alır veya ayarlar . Oluşturulan projenin bir sayfaya sığabilmesi için sayfa boyutu değiştirilir. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Özet görev çubuğundaki alt görevlerin işaretlenmesi gerekip gerekmediğini belirten bir değer alır veya ayarlar. Alt görevler için, Toplama alanı, alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını belirtir. Özet görevler için, Toplama alanı, özet görev çubuğunun toplanmış çubuklar gösterip göstermediğini gösterir. Herhangi bir alt görevin bunları toplaması için Özet görevler için Topla alanını Evet olarak ayarlamış olmanız gerekir. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Oluşturmaya başlamak için tarihi alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Gantt şeması ve Görev Sayfası grafiğindeki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı çizelgelerinde oluşturulan görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Örneklerin listesini alır veya ayarlar.[`TextStyle`](../../aspose.tasks.visualization/textstyle) proje görünümünde görünen sınıf. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Alır veya ayarlar[`Timescale`](../saveoptions/timescale) proje grafik biçiminde kaydedildiğinde zaman ölçeğinin (varsa) nasıl oluşturulacağını kontrol etmek için kullanılan değer. |
| override [UseGradientBrush](../../aspose.tasks.saving/svgoptions/usegradientbrush) { get; set; } | Proje düzenini oluştururken degrade fırçasının kullanılıp kullanılmayacağını belirler. Şu anda degrade fırçasının kullanımı, SVG'ye işleme için desteklenmiyor. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | İşlenecek görünüm sütunlarının bir listesini alır veya ayarlar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). Ayarlanmadıysa, görev kimlikleri, görev adları, başlangıç ve bitiş yalnızca oluşturulur. Hem Görünüm hem de[`ViewSettings`](../saveoptions/viewsettings) özellikler ayarlandığında, Görünüm'deki sütunlar, ViewSettings'deki sütunları geçersiz kılar. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Bir görünüm alır veya ayarlar ([`View`](../saveoptions/view) işlemek için. Hangi görünümün PDF, HTML veya Görüntü biçimlerine kaydedileceğini açıkça belirtmek için bu seçenekleri kullanabilirsiniz. Bu özellik ayarlanırsa,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) proje kaydedildiğinde özellik yok sayılır. Görünüm aşağıdaki ekranlardan birinden olmalıdır (([`Screen`](../../aspose.tasks/view/screen) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Ayrıca bakınız

* class [SaveOptions](../saveoptions)
* ad alanı [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* toplantı [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
