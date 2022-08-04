---
title: PdfSaveOptions
second_title: Aspose.Tasks for .NET API Referansı
description: Proje sayfalarını PDFye dönüştürürken ek seçenekleri belirlemeye izin verir.
type: docs
weight: 1850
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Proje sayfalarını PDF'ye dönüştürürken ek seçenekleri belirlemeye izin verir.

```csharp
public class PdfSaveOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Yeni bir örneğini başlatır[`PdfSaveOptions`](../pdfsaveoptions)bir belgeyi kaydetmek için kullanılabilecek sınıf[`PDF`](../savefileformat) biçim. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Örneklerin listesini alır veya ayarlar.[`BarStyle`](../../aspose.tasks.visualization/barstyle) proje görünümünde görünen sınıf. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance) { get; set; } | Oluşturulan PDF belgesi için istenen uyumluluk düzeyini alır veya ayarlar. VarsayılanPdf15 . |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Özel sayfa boyutunu punto cinsinden alır veya ayarlar (1 nokta = 1/72 inç). |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname) { get; set; } | Oluşturma için varsayılan yazı tipini alır veya ayarlar. |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails) { get; set; } | Dijital imza ayrıntılarını alır veya ayarlar. Ayarlanmazsa, imzalama gerçekleştirilmez. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Çalışma dışı zamanın çizilmesi gerekip gerekmediğini belirten bir değer alır veya ayarlar (Varsayılan değer DOĞRU'dur). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails) { get; set; } | Bir şifreleme ayrıntısı alır veya ayarlar. Ayarlanmazsa şifreleme yapılmaz. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Oluşturmayı bitirmek için bir tarih alır veya ayarlar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Satır yüksekliğinin içeriğine uyacak şekilde artırılması gerekip gerekmediğini belirten bir değer alır veya ayarlar. |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback) { get; set; } | Çözümlenen yazı tiplerini özelleştirmek için kullanılabilecek bir geri arama alır veya ayarlar. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Bir liste alır veya ayarlar[`Gridline`](../../aspose.tasks.visualization/gridline) proje görünümünde görünen. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Göstergenin her sayfada gösterilip gösterilmeyeceğini belirten bir değer alır veya ayarlar (Varsayılan değer DOĞRU'dur). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Kritik görevlerin kırmızı renkte görüntülenip görüntülenmeyeceğini belirten bir değer alır veya ayarlar (Varsayılan değer YANLIŞ'tır). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Çalışmayan zaman rengini alır veya ayarlar. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Projenin sayfa sayısını alır veya ayarlar. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages) { get; set; } | Proje düzenini ayrı dosyalara kaydederken kaydedilecek sayfa numaralarının listesini alır veya ayarlar. Bu liste boşsa tüm sayfalar kaydedilecektir. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback) { get; set; } | Oluşturulan her sayfa için bir çıktı akışı almak için kullanılan kullanıcı tanımlı bir geri aramayı alır veya ayarlar. Şu durumlarda uygulanabilir:[`SaveToSeparateFiles`](./savetoseparatefiles) seçenek kullanılır. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | İşlenecek sayfanın boyutunu alır veya ayarlar (Varsayılan değer PageSize.A4'tür). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Alır veya ayarlar[`PresentationFormat`](../saveoptions/presentationformat) belgenin kaydedileceği yer. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap) { get; set; } | Son görev ile alt bilgi arasındaki boşluğun azaltılması gerekip gerekmediğini belirten bir değer alır veya ayarlar. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Proje grafik biçiminde kaydedildiğinde, projenin tek bir sayfaya dönüştürülüp dönüştürülmeyeceğini belirten bir değer alır veya ayarlar . Oluşturulan projenin bir sayfaya sığabilmesi için sayfa boyutu değiştirilir. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Özet görev çubuğundaki alt görevlerin işaretlenmesi gerekip gerekmediğini belirten bir değer alır veya ayarlar. Alt görevler için, Toplama alanı, alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını belirtir. Özet görevler için, Toplama alanı, özet görev çubuğunun toplanmış çubuklar gösterip göstermediğini gösterir. Herhangi bir alt görevin bunları toplaması için Özet görevler için Topla alanını Evet olarak ayarlamış olmanız gerekir. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles) { get; set; } | Proje sayfalarının ayrı dosyalara kaydedilip kaydedilmeyeceğini belirten bir değer alır veya ayarlar. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Oluşturmaya başlamak için tarihi alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Gantt şeması ve Görev Sayfası grafiğindeki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı çizelgelerinde oluşturulan görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression) { get; set; } | Görüntüler hariç tüm içerik akışları için kullanılacak bir sıkıştırma türünü alır veya ayarlar. VarsayılanFlate . |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Örneklerin listesini alır veya ayarlar.[`TextStyle`](../../aspose.tasks.visualization/textstyle) proje görünümünde görünen sınıf. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Alır veya ayarlar[`Timescale`](../saveoptions/timescale) proje grafik biçiminde kaydedildiğinde zaman ölçeğinin (varsa) nasıl oluşturulacağını kontrol etmek için kullanılan değer. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Gantt Grafiği oluşturulurken degrade fırçasının kullanılması gerekip gerekmediğini belirten bir değer alır veya ayarlar. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont) { get; set; } | Oluşturma için varsayılan yazı tipinin kullanılması gerekip gerekmediğini belirten bir değer alır veya ayarlar. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | İşlenecek görünüm sütunlarının bir listesini alır veya ayarlar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). Ayarlanmadıysa, görev kimlikleri, görev adları, başlangıç ve bitiş yalnızca oluşturulur. Hem Görünüm hem de[`ViewSettings`](../saveoptions/viewsettings) özellikler ayarlandığında, Görünüm'deki sütunlar, ViewSettings'deki sütunları geçersiz kılar. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Bir görünüm alır veya ayarlar ([`View`](../saveoptions/view) işlemek için. Hangi görünümün PDF, HTML veya Görüntü biçimlerine kaydedileceğini açıkça belirtmek için bu seçenekleri kullanabilirsiniz. Bu özellik ayarlanırsa,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) proje kaydedildiğinde özellik yok sayılır. Görünüm aşağıdaki ekranlardan birinden olmalıdır (([`Screen`](../../aspose.tasks/view/screen) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Ayrıca bakınız

* class [SaveOptions](../saveoptions)
* ad alanı [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* toplantı [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->