---
title: "SaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bu, bir projeyi belirli bir formata kaydederken kullanıcının ek seçenekler belirtmesine izin veren sınıflar için soyut bir temel sınıftır."
type: docs
weight: 274
url: /tr/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Bu, bir projeyi belirli bir formata kaydederken kullanıcının ek seçenekler belirtmesine izin veren sınıflar için soyut bir temel sınıftır.

--------------------

SaveOptions sınıfından türetilen herhangi bir sınıfın örneği, bir belge kaydedilirken kullanıcıya özel seçenekler tanımlaması için akış Save veya string Save aşırı yüklemelerine geçirilir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Proje görünümünde görünen [BarStyle](../../com.aspose/tasks/barstyle) sınıfının örneklerinin listesini alır. |
| [getCustomPageSize()](#getCustomPageSize--) | Özel sayfa boyutunu nokta cinsinden alır (1 nokta = inçin 1/72'si). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değeri alır (Varsayılan değer TRUE'dur). |
| [getEndDate()](#getEndDate--) | Render işleminin tamamlanacağı tarihi alır. |
| [getFitContent()](#getFitContent--) | Satır yüksekliğinin içeriğine uyması için artırılıp artırılmayacağını gösteren bir değeri alır. |
| [getGridlines()](#getGridlines--) | Proje görünümünde görünen [Gridline](../../com.aspose/tasks/gridline) listesini alır. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Lejantın nasıl render edileceğini tanımlayan bir değeri alır. |
| [getLegendItems()](#getLegendItems--) | Sayfa lejantında hangi çubukların render edileceğini tanımlayan PageLegendItem dizisini alır. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri alır (Varsayılan değer FALSE'dur). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Çalışma dışı zaman rengini alır. |
| [getPageCount()](#getPageCount--) | Projenin sayfa sayısını alır. |
| [getPageSize()](#getPageSize--) | Render edilecek sayfanın boyutunu alır (Varsayılan değer PageSize.A4'tür). |
| [getPresentationFormat()](#getPresentationFormat--) | Belgenin kaydedileceği `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) değerini alır. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Proje grafik formatta kaydedildiğinde tek bir sayfaya render edilip edilmeyeceğini gösteren bir değeri alır. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini gösteren bir değeri alır. |
| [getStartDate()](#getStartDate--) | Render etmeye başlanacak tarihi alır. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Görev bağlantılarının render edilmesinin bazı yönlerini özelleştirmek için kullanılabilecek bir geri çağırma alır. |
| [getTextStyles()](#getTextStyles--) | Proje görünümünün render edilmesi sırasında uygulanan metin stillerinin listesini alır. |
| [getTimescale()](#getTimescale--) | `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) değerini alır; bu değer, proje grafik formatta kaydedildiğinde zaman ölçeğinin (varsa) nasıl render edileceğini kontrol etmek için kullanılır. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Zaman ölçeğinin sağ ucunun sayfa sonuyla nasıl hizalanacağını tanımlayan davranışı alır. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Gantt Şeması render edilirken degrade fırçasının kullanılıp kullanılmayacağını gösteren bir değeri alır. |
| [getView()](#getView--) | Render edilecek görünüm sütunlarının listesini alır ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Render edilecek bir görünümü (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) alır. |
| [isPortrait()](#isPortrait--) | Sayfa yönünün dikey olup olmadığını gösteren bir değer alır; sayfa yönü yataysa false döndürür. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Proje görünümünde görünen [BarStyle](../../com.aspose.tasks/barstyle) sınıfının örneklerinin listesini ayarlar. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Özel sayfa boyutunu puan cinsinden ayarlar (1 puan = 1/72 inç). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değeri ayarlar (Varsayılan değer TRUE'dur). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Render işleminin bitirileceği tarihi ayarlar. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Satır yüksekliğinin içeriğe sığacak şekilde artırılıp artırılmayacağını gösteren bir değeri ayarlar. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Proje görünümünde görünen [Gridline](../../com.aspose.tasks/gridline) öğelerinin listesini ayarlar. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Bir lejantın nasıl render edileceğini tanımlayan bir değeri ayarlar. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Sayfa lejantında hangi çubukların render edileceğini tanımlayan PageLegendItem dizisini ayarlar. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri ayarlar (Varsayılan değer FALSE'dur). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Çalışma dışı zaman rengini ayarlar. |
| [setPageSize(int value)](#setPageSize-int-) | Render edilecek sayfanın boyutunu ayarlar (Varsayılan değer PageSize.A4'tür). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Sayfa yönünün dikey olup olmadığını gösteren bir değeri ayarlar; sayfa yönü yataysa false döndürür. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Belgenin kaydedileceği `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) değerini ayarlar. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Proje grafik formatta kaydedildiğinde tek bir sayfaya render edilip edilmeyeceğini gösteren bir değeri ayarlar. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini gösteren bir değeri ayarlar. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Renderlemeye başlanacak tarihi ayarlar. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Görev bağlantılarının renderlenmesinin bazı yönlerini özelleştirmek için kullanılabilecek bir geri aramayı ayarlar. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Proje görünümünün renderlenmesi sırasında uygulanan metin stillerinin listesini ayarlar. |
| [setTimescale(int value)](#setTimescale-int-) | Renderleme sırasında zaman ölçeğinin (varsa) nasıl görüntüleneceğini kontrol etmek için kullanılan `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) değerini ayarlar. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Zaman ölçeğinin sağ ucunun sayfa sonuna nasıl hizalanacağını tanımlayan bir davranışı ayarlar. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Gantt Şeması renderlenirken degrade fırçasının kullanılıp kullanılmayacağını gösteren bir değeri ayarlar. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Renderlenecek görünüm sütunlarının listesini ayarlar ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Renderlenecek bir görünümü (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) ayarlar. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Proje görünümünde görünen [BarStyle](../../com.aspose/tasks/barstyle) sınıfının örneklerinin listesini alır.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - proje görünümünde görünen [BarStyle](../../com.aspose.tasks/barstyle) sınıfının örneklerinin listesi.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Özel sayfa boyutunu nokta cinsinden alır (1 nokta = inçin 1/72'si).

**Returns:**
java.awt.geom.Dimension2D - puan cinsinden özel sayfa boyutu (1 puan = 1/72 inç).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değeri alır (Varsayılan değer TRUE'dur).

**Returns:**
boolean - çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değer (Varsayılan değer TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Render işleminin tamamlanacağı tarihi alır.

**Returns:**
java.util.Date - renderlemenin tamamlanacağı tarih.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Satır yüksekliğinin içeriğine uyması için artırılıp artırılmayacağını gösteren bir değeri alır.

**Returns:**
boolean - satır yüksekliğinin içeriğine uyması için artırılıp artırılmayacağını gösteren bir değer.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Proje görünümünde görünen [Gridline](../../com.aspose/tasks/gridline) listesini alır.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - proje görünümünde görünen [Gridline](../../com.aspose.tasks/gridline) listesidir.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Bir lejandın nasıl renderleneceğini tanımlayan bir değeri alır. Varsayılan değer LegendDrawingOptions.OnEveryPage.

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Returns:**
int - bir lejandın nasıl renderleneceğini tanımlayan bir değer.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Sayfa lejandında hangi çubukların renderleneceğini tanımlayan PageLegendItem dizisini alır. Null ise, varsayılan öğeler renderlenir.

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Returns:**
com.aspose.tasks.PageLegendItem[] - sayfa lejandında hangi çubukların renderleneceğini tanımlayan PageLegendItem dizisi.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri alır (Varsayılan değer FALSE'dur).

**Returns:**
boolean - kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değer (Varsayılan değer FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Çalışma dışı zaman rengini alır.

**Returns:**
java.awt.Color - çalışma dışı zaman rengi.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Projenin sayfa sayısını alır.

**Returns:**
int - projenin sayfa sayısı.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Render edilecek sayfanın boyutunu alır (Varsayılan değer PageSize.A4'tür).

**Returns:**
int - renderlenecek sayfanın boyutu (Varsayılan değer PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Belgenin kaydedileceği `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) değerini alır.

**Returns:**
int - belgenin kaydedileceği `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)).
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Proje grafik formatta kaydedildiğinde tek bir sayfaya render edilip edilmeyeceğini gösteren bir değeri alır. Sayfa boyutu, renderlenen projenin bir sayfaya sığabilmesi için değiştirilecektir.

**Returns:**
boolean - bir projenin grafik formatında kaydedildiğinde tek bir sayfaya render edilip edilmeyeceğini belirten bir değer.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini belirten bir değer alır. Alt görevler için Rollup alanı, alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını gösterir. Özet görevler için Rollup alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Alt görevlerin onlara toplanabilmesi için özet görevler için Rollup alanının Evet olarak ayarlanmış olması gerekir.

--------------------

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Returns:**
boolean - özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini belirten bir değer.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Render etmeye başlanacak tarihi alır.

**Returns:**
java.util.Date - renderlamaya başlanacak tarih.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Görev bağlantılarının render edilmesinin bazı yönlerini özelleştirmek için kullanılabilecek bir geri çağırma alır.

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Proje görünümünün render edilmesi sırasında uygulanan metin stillerinin listesini alır.

--------------------

Bu stiller, GanttCharView.setTextStyles ile tanımlanan stillerin üzerine yazar.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - bir proje görünümünün renderlanması sırasında uygulanan metin stillerinin listesi.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


`Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) değerini alır; bu değer, proje grafik formatta kaydedildiğinde zaman ölçeğinin (varsa) nasıl render edileceğini kontrol etmek için kullanılır.

**Returns:**
int - proje grafik formatında kaydedildiğinde zaman ölçeğinin (varsa) nasıl renderlanacağını kontrol etmek için kullanılan `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) değeri.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Zaman ölçeğinin sağ ucunun sayfa sonuyla nasıl hizalanacağını tanımlayan davranışı alır.

**Returns:**
int - zaman ölçeğinin sağ ucunun sayfa sonuyla nasıl hizalanacağını tanımlayan bir davranış.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Gantt Şeması render edilirken degrade fırçasının kullanılıp kullanılmayacağını gösteren bir değeri alır.

--------------------

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Returns:**
boolean - Gantt Şeması renderlanırken degrade fırçasının kullanılıp kullanılmayacağını belirten bir değer.
### getView() {#getView--}
```
public final ProjectView getView()
```


Renderlanacak görünüm sütunlarının listesini alır ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Ayarlanmamışsa yalnızca görev kimlikleri, görev adları, başlangıç ve bitiş renderlanır. Hem View hem de `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) özellikleri ayarlıysa, View'tan gelen sütunlar ViewSettings'ten gelen sütunların üzerine yazar.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Renderlanacak bir görünüm (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) alır. Bu seçeneği, hangi görünümün PDF, HTML veya Image formatlarında kaydedileceğini açıkça belirtmek için kullanabilirsiniz. Bu özellik ayarlıysa, proje kaydedildiğinde [PresentationFormat](../../com.aspose.tasks/presentationformat) özelliği yoksayılır. Görünüm, aşağıdaki ekranlardan biri olmalıdır ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Sayfa yönünün dikey olup olmadığını gösteren bir değer alır; sayfa yönü yataysa false döndürür.

--------------------

SaveOptions.getPageSize() == PageSize.DefinedInView olduğunda uygulanmaz. Bu durumda yerine [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) kullanılır. [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) ayarlıysa da uygulanmaz.

**Returns:**
boolean - sayfa yönünün portre olup olmadığını gösteren bir değer; sayfa yönü manzara ise false döndürür.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Proje görünümünde görünen [BarStyle](../../com.aspose.tasks/barstyle) sınıfının örneklerinin listesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | proje görünümünde görünen [BarStyle](../../com.aspose.tasks/barstyle) sınıfının örneklerinin listesi. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Özel sayfa boyutunu puan cinsinden ayarlar (1 puan = 1/72 inç).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.geom.Dimension2D | nokta cinsinden özel sayfa boyutu (1 nokta = inçin 1/72'si). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Çalışma dışı zamanın çizilip çizilmeyeceğini gösteren bir değeri ayarlar (Varsayılan değer TRUE'dur).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | çalışma dışı zamanın çizilip çizilmeyeceğini belirten bir değer (Varsayılan değer TRUE'dur). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Render işleminin bitirileceği tarihi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | renderlamanın sonlandırılacağı tarih. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Satır yüksekliğinin içeriğe sığacak şekilde artırılıp artırılmayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | satır yüksekliğinin içeriğine uyacak şekilde artırılıp artırılmayacağını belirten bir değer. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Proje görünümünde görünen [Gridline](../../com.aspose.tasks/gridline) öğelerinin listesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | proje görünümünde görünen [Gridline](../../com.aspose.tasks/gridline) öğelerinin listesi. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Bir lejandın nasıl renderlanacağını tanımlayan bir değer ayarlar. Varsayılan değer LegendDrawingOptions.OnEveryPage'dir.

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Lejandın nasıl renderlanacağını tanımlayan bir değer. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Sayfa lejandında hangi çubukların renderlanacağını tanımlayan PageLegendItem dizisini ayarlar. Null ise, varsayılan öğeler renderlanır.

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | Sayfa lejandında hangi çubukların renderlanacağını tanımlayan PageLegendItem dizisi. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri ayarlar (Varsayılan değer FALSE'dur).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değer (Varsayılan değer FALSE'tur). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Çalışma dışı zaman rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | çalışma dışı zaman rengi. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Render edilecek sayfanın boyutunu ayarlar (Varsayılan değer PageSize.A4'tür).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | renderlanacak sayfanın boyutu (Varsayılan değer PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Sayfa yönünün dikey olup olmadığını gösteren bir değeri ayarlar; sayfa yönü yataysa false döndürür.

--------------------

SaveOptions.PageSize == Visualization.PageSize.DefinedInView olduğunda uygulanmaz. Bu durumda [PageSettings.setPortrait(boolean)](../../com.aspose/tasks/pagesettings\#setPortrait-boolean-) kullanılır. [getCustomPageSize()](../../com.aspose/tasks/saveoptions\#getCustomPageSize--) ayarlandığında uygulanmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | sayfa yönünün portre olup olmadığını gösteren bir değer; sayfa yönü manzara ise false döndürür. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Belgenin kaydedileceği `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | int | belgenin kaydedileceği `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)). |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Projeyi grafik formatında kaydederken tek bir sayfaya render edilip edilmeyeceğini belirten bir değer ayarlar. Sayfa boyutu, render edilen projenin tek sayfaya sığabilmesi için değiştirilecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Projeyi grafik formatında kaydederken tek bir sayfaya render edilip edilmeyeceğini belirten bir değer. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini belirten bir değer ayarlar. Alt görevler için Rollup alanı, alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını gösterir. Özet görevler için Rollup alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Alt görevlere toplanabilmesi için özet görevlerin Rollup alanının Evet olarak ayarlanmış olması gerekir.

--------------------

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini belirten bir değer. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Renderlemeye başlanacak tarihi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | renderlamaya başlanacak tarih. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Görev bağlantılarının renderlenmesinin bazı yönlerini özelleştirmek için kullanılabilecek bir geri aramayı ayarlar.

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | görev bağlantılarının render edilmesinin bazı yönlerini özelleştirmek için kullanılabilecek bir geri çağırma. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Proje görünümünün renderlenmesi sırasında uygulanan metin stillerinin listesini ayarlar.

--------------------

Bu stiller, GanttCharView.setTextStyles ile tanımlanan stillerin üzerine yazar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | bir proje görünümünün render edilmesi sırasında uygulanan metin stillerinin listesi. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Renderleme sırasında zaman ölçeğinin (varsa) nasıl görüntüleneceğini kontrol etmek için kullanılan `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | int | `Timescale`([getTimescale()](../../com.aspose/tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose/tasks/saveoptions\#setTimescale-int-)) değeri, proje grafik formatında kaydedildiğinde zaman ölçeğinin (varsa) nasıl render edileceğini kontrol etmek için kullanılır. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Zaman ölçeğinin sağ ucunun sayfa sonuna nasıl hizalanacağını tanımlayan bir davranışı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | zaman ölçeğinin sağ ucunun sayfa sonuyla nasıl hizalanacağını tanımlayan bir davranış. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Gantt Şeması renderlenirken degrade fırçasının kullanılıp kullanılmayacağını gösteren bir değeri ayarlar.

--------------------

Yalnızca Gantt şema görünümü renderlendiğinde uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Gantt Şeması render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirten bir değer. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Render edilecek görünüm sütunlarının bir listesini ayarlar ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Ayarlanmamışsa yalnızca görev kimlikleri, görev adları, başlangıç ve bitiş render edilir. Hem View hem de `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) özellikleri ayarlanmışsa, View'dan gelen sütunlar ViewSettings'teki sütunların üzerine yazar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | render edilecek görünüm sütunlarının listesi ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


render etmek için bir görünüm (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) ayarlar. Bu seçeneği, hangi görünümün PDF, HTML veya Image formatlarında kaydedileceğini açıkça belirtmek için kullanabilirsiniz. Bu özellik ayarlanırsa, proje kaydedildiğinde [PresentationFormat](../../com.aspose.tasks/presentationformat) özelliği göz ardı edilir. Görünüm, aşağıdaki ekranlardan biri olmalıdır ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | render etmek için bir görünüm (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))). |

