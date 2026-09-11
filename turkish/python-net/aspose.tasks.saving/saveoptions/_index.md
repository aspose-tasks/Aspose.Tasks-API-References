---
title: "SaveOptions"
second_title: "Aspose.Tasks for Python via .NET API Referansı"
description: 
type: docs
weight: 130
url: /tr/python-net/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

Bu, bir projenin belirli bir formata kaydedilirken kullanıcının ek seçenekler belirtmesine izin veren sınıflar için soyut bir temel sınıftır<br/>            belirli bir formata.

SaveOptions türü aşağıdaki üyeleri ortaya çıkar:
## Özellikler
| Ad | Açıklama |
| :- | :- |
| save_format | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| bar_styles | Proje görünümünde görünen [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) sınıfının örneklerinin listesini alır veya ayarlar. |
| draw_non_working_time | Çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değeri alır veya ayarlar (Varsayılan değer TRUE'dur). |
| end_date | Renderlamayı bitirmek için bir tarihi alır veya ayarlar. |
| timescale_fit_behavior | Zaman ölçeğinin sağ ucunu sayfa sonuyla hizalamanın nasıl yapılacağını tanımlayan bir davranışı alır veya ayarlar. |
| fit_content | Satır yüksekliğinin içeriğine sığacak şekilde artırılıp artırılmayacağını gösteren bir değeri alır veya ayarlar. |
| gridlines | Proje görünümünde görünen [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) listesini alır veya ayarlar. |
| legend_drawing_options | Bir lejandın nasıl render edileceğini tanımlayan bir değeri alır veya ayarlar. Varsayılan değer LegendDrawingOptions.OnEveryPage'dir. |
| legend_items | Sayfa lejandında hangi çubukların render edileceğini tanımlayan PageLegendItem dizisini alır veya ayarlar.<br/>            Eğer null ise, varsayılan öğeler render edilir. |
| mark_critical_tasks | Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar (Varsayılan değer FALSE'tur). |
| non_working_time_color | Çalışma dışı zaman rengini alır veya ayarlar. |
| page_count | Projenin sayfa sayısını alır veya ayarlar. |
| page_size | Render edilecek sayfanın boyutunu alır veya ayarlar (Varsayılan değer PageSize.A4'tür). |
| is_portrait | Sayfa yönünün portre olup olmadığını belirten bir değeri alır veya ayarlar; sayfa yönü yatay ise false döner. |
| presentation_format | Belgenin kaydedileceği [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) değerini alır veya ayarlar. |
| roll_up_gantt_bars | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini belirten bir değeri alır veya ayarlar.<br/>            Alt görevler için, Rollup alanı alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını gösterir.<br/>            Özet görevler için, Rollup alanı özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir.<br/>            Alt görevlerin onlara toplanabilmesi için, özet görevler için Rollup alanının Yes olarak ayarlanmış olması gerekir. |
| start_date | Render etmeye başlanacak tarihi alır veya ayarlar. |
| text_styles | Proje görünümünün render edilmesi sırasında uygulanan metin stilleri listesini alır veya ayarlar. |
| timescale | Proje grafik formatta kaydedildiğinde zaman ölçeğinin (varsa) nasıl render edileceğini kontrol etmek için kullanılan [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) değerini alır veya ayarlar. |
| use_gradient_brush | Gantt Şeması render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirten bir değeri alır veya ayarlar. |
| view | Render edilecek görünüm sütunlarının listesini alır veya ayarlar ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Ayarlanmamışsa yalnızca görev kimlikleri, görev adları, başlangıç ve bitiş render edilir.<br/>            Hem View hem de [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) özellikleri ayarlanmışsa, View'ten gelen sütunlar ViewSettings'ten gelen sütunların üzerine yazar. |
| view_settings | Render edilecek bir görünümü ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) alır veya ayarlar. Bu seçeneği, hangi görünümün PDF, HTML veya Image formatlarında kaydedileceğini açıkça belirtmek için kullanabilirsiniz.<br/>            Bu özellik ayarlanmışsa, proje kaydedildiğinde [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) özelliği yoksayılır.<br/>            Görünüm, aşağıdaki ekranlardan biri olmalıdır (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Özel sayfa boyutunu nokta cinsinden alır veya ayarlar (1 nokta = inçin 1/72'si). |
| render_to_single_page | Bir projenin tek bir sayfaya render edilip edilmemesini belirten bir değeri alır veya ayarlar<br/>            proje grafik formatında kaydedildiğinde.<br/>            Sayfa boyutu, render edilen projenin tek bir sayfaya sığabilmesi için değiştirilecektir. |

### Ayrıca Bakınız

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

