---
title: "Aspose::Tasks::Saving::SaveOptions class"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "C++ için Aspose.Tasks"
description: "Bu, bir projeyi belirli bir biçimde kaydederken kullanıcıya ek seçenekler belirtme imkanı tanıyan sınıflar için soyut bir temel sınıftır."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

Bu, bir projeyi belirli bir biçimde kaydederken kullanıcıya ek seçenekler belirtme imkanı tanıyan sınıflar için soyut bir temel sınıftır.

SaveOptions sınıfından türetilen herhangi bir sınıfın örneği, bir belgeyi kaydederken kullanıcıya özel seçenekler tanımlaması için akış Save veya string Save aşırı yüklemelerine geçirilir.

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | Proje görünümünde görünen BarStyle sınıfının örneklerinin listesini alır. |
| [get_CustomPageSize](./get_custompagesize/) | Özel sayfa boyutunu puan cinsinden alır (1 puan = inçin 1/72'si). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | Çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değeri alır (Varsayılan değer TRUE'dır). |
| [get_EndDate](./get_enddate/) | Render işleminin sonlandırılacağı tarihi alır. |
| [get_FitContent](./get_fitcontent/) | Satır yüksekliğinin içeriğe sığacak şekilde artırılıp artırılmayacağını gösteren bir değeri alır. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | Bir görünümün takvim bölümünün son sayfanın sonuna (sağ tarafına) render edilip edilmediğini alır. Değer false ise, takvim bölümü boş bir alan olsa bile tam olarak EndDate'e render edilir. |
| [get_Gridlines](./get_gridlines/) | Proje görünümünde görünen Gridline (ızgara çizgileri) listesini alır. |
| [get_IsPortrait](./get_isportrait/) | Sayfa yönünün dikey olup olmadığını gösteren bir değeri alır; sayfa yönü yataysa false döndürür. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | Bir lejantın nasıl render edileceğini tanımlayan bir değeri alır. Varsayılan değer LegendDrawingOptions.OnEveryPage'dir. |
| [get_LegendItems](./get_legenditems/) | Sayfa lejantında hangi çubukların render edileceğini tanımlayan PageLegendItem dizisini alır. Null ise, varsayılan öğeler render edilir. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri alır (Varsayılan değer FALSE'tır). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | Çalışma dışı zaman rengini alır. |
| [get_PageCount](./get_pagecount/) | Projenin sayfa sayısını alır. |
| [get_PageSize](./get_pagesize/) | Render edilecek sayfanın boyutunu alır (Varsayılan değer PageSize.A4'tür). |
| [get_PresentationFormat](./get_presentationformat/) | Belgenin kaydedileceği PresentationFormat'ı alır. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | Proje grafik formatında kaydedildiğinde tek bir sayfaya render edilip edilmeyeceğini gösteren bir değeri alır. Sayfa boyutu, render edilen projenin tek sayfaya sığacak şekilde değiştirilecektir. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini gösteren bir değeri alır. Alt görevler için Rollup alanı, alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını gösterir. Özet görevler için Rollup alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Alt görevlerin onlara toplanabilmesi için özet görevlerde Rollup alanının Yes olarak ayarlanmış olması gerekir. |
| [get_StartDate](./get_startdate/) | Render işlemine başlanacak tarihi alır. |
| [get_TextStyles](./get_textstyles/) | Proje görünümünün render edilmesi sırasında uygulanan metin stilleri listesini alır. |
| [get_Timescale](./get_timescale/) | Proje grafik formatında kaydedildiğinde zaman ölçeğinin (varsa) nasıl render edileceğini kontrol etmek için kullanılan Timescale değerini alır. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | Zaman ölçeğinin sağ ucunun sayfa sonuna nasıl hizalanacağını tanımlayan bir davranışı alır. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Gantt Şeması render edilirken gradient fırçasının kullanılıp kullanılmayacağını gösteren bir değeri alır. |
| [get_View](./get_view/) | Render edilecek görünüm sütunlarının listesini alır (GanttChartColumn). Ayarlanmamışsa yalnızca görev kimlikleri, görev adları, başlangıç ve bitiş render edilir. Hem View hem de ViewSettings özellikleri ayarlıysa, View'tan gelen sütunlar ViewSettings'ten gelen sütunların üzerine yazar. |
| [get_ViewSettings](./get_viewsettings/) | Render edilecek bir görünüm (View) alır. Bu seçeneği, hangi görünümün PDF, HTML veya Image formatlarında kaydedileceğini açıkça belirtmek için kullanabilirsiniz. Bu özellik ayarlıysa, proje kaydedilirken Visualization::PresentationFormat özelliği yok sayılır. Görünüm, aşağıdaki ekranlardan biri olmalıdır ((Aspose::Tasks::View::Screen)): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |
| [set_BarStyles](./set_barstyles/) | Proje görünümünde görünen BarStyle sınıfının örneklerinin listesini ayarlar. |
| [set_CustomPageSize](./set_custompagesize/) | Özel sayfa boyutunu puan cinsinden ayarlar (1 puan = inçin 1/72'si). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | Çalışmayan zamanın çizilmesi gerektiğini gösteren bir değer ayarlar (Varsayılan değer TRUE'dur). |
| [set_EndDate](./set_enddate/) | Render işleminin tamamlanacağı tarihi ayarlar. |
| [set_FitContent](./set_fitcontent/) | Satır yüksekliğinin içeriğine uyması için artırılması gerektiğini gösteren bir değer ayarlar. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | Bir görünümün takvim bölümünün son sayfanın sonuna (sağ tarafına) render edilip edilmeyeceğini ayarlar. Değer false ise, takvim bölümü boş bir alan olsa bile tam olarak EndDate'e render edilir. |
| [set_Gridlines](./set_gridlines/) | Proje görünümünde görünen Gridline listesini ayarlar. |
| [set_IsPortrait](./set_isportrait/) | Sayfa yönünün portre olup olmadığını gösteren bir değer ayarlar; sayfa yönü manzara ise false döndürür. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | Bir lejantın nasıl render edileceğini tanımlayan bir değer ayarlar. Varsayılan değer LegendDrawingOptions.OnEveryPage'dir. |
| [set_LegendItems](./set_legenditems/) | Sayfa lejantında hangi çubukların render edileceğini tanımlayan PageLegendItem dizisini ayarlar. Null ise, varsayılan öğeler render edilir. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değer ayarlar (Varsayılan değer FALSE'tır). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | Çalışmayan zaman rengini ayarlar. |
| [set_PageSize](./set_pagesize/) | Render edilecek sayfanın boyutunu ayarlar (Varsayılan değer PageSize.A4'tür). |
| [set_PresentationFormat](./set_presentationformat/) | Belgenin kaydedileceği PresentationFormat'ı ayarlar. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | Proje grafik formatında kaydedildiğinde tek bir sayfaya render edilip edilmeyeceğini gösteren bir değer ayarlar. Sayfa boyutu, render edilen projenin tek sayfaya sığması için değiştirilecektir. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini gösteren bir değer ayarlar. Alt görevler için Rollup alanı, alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını gösterir. Özet görevler için Rollup alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Alt görevlerin toplanabilmesi için özet görevlerde Rollup alanının Yes olarak ayarlanmış olması gerekir. |
| [set_StartDate](./set_startdate/) | Render işlemine başlanacak tarihi ayarlar. |
| [set_TextStyles](./set_textstyles/) | Proje görünümünün render edilmesi sırasında uygulanan metin stilleri listesini ayarlar. |
| [set_Timescale](./set_timescale/) | Proje grafik formatında kaydedildiğinde zaman ölçeğinin (varsa) nasıl render edileceğini kontrol etmek için kullanılan Timescale değerini ayarlar. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | Zaman ölçeğinin sağ ucunun sayfa sonuna nasıl hizalanacağını tanımlayan bir davranışı ayarlar. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Gantt Şeması render edilirken gradient fırçasının kullanılıp kullanılmayacağını gösteren bir değer ayarlar. |
| [set_View](./set_view/) | Render edilecek görünüm sütunlarının listesini ayarlar ( GanttChartColumn ). Ayarlanmazsa yalnızca görev kimlikleri, görev adları, başlangıç ve bitiş render edilir. Hem View hem de ViewSettings özellikleri ayarlıysa, View'tan gelen sütunlar ViewSettings'ten gelenleri geçersiz kılar. |
| [set_ViewSettings](./set_viewsettings/) | Render edilecek bir görünüm ( View ) ayarlar. Bu seçeneği, hangi görünümün PDF, HTML veya Image formatlarında kaydedileceğini açıkça belirtmek için kullanabilirsiniz. Bu özellik ayarlıysa, proje kaydedildiğinde Visualization::PresentationFormat özelliği yok sayılır. Görünüm, aşağıdaki ekranlardan biri olmalıdır (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

