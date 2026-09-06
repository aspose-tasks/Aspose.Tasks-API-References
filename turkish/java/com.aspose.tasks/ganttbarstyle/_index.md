---
title: "GanttBarStyle"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Gantt Şema görünümünde MSP tarafından kullanılan bir çubuk stilini temsil eder."
type: docs
weight: 109
url: /tr/java/com.aspose.tasks/ganttbarstyle/
---

**Inheritance:**
java.lang.Object
```
public class GanttBarStyle
```

Gantt Şema görünümünde MSP tarafından kullanılan bir çubuk stilini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GanttBarStyle()](#GanttBarStyle--) | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | Görevin çubuğunun alt kısmında render edilecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. |
| [getBottomField()](#getBottomField--) | Çubuğun alt kısmında gösterilecek veriyi alır. |
| [getEndShape()](#getEndShape--) | Çubuğun son şekli alır. |
| [getEndShapeColor()](#getEndShapeColor--) | Son şeklin rengini alır. |
| [getEndShapeType()](#getEndShapeType--) | Son şeklin tipini alır. |
| [getFrom()](#getFrom--) | Gantt çubuğunun başlangıç noktası konumunu alır. |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | Görevin çubuğunun içinde render edilecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. |
| [getInsideField()](#getInsideField--) | Çubuğun içinde gösterilecek veriyi alır. |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | Görevin çubuğunun sol tarafında render edilecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. |
| [getLeftField()](#getLeftField--) | Çubuğun sol tarafında gösterilecek veriyi alır. |
| [getMiddleFillPattern()](#getMiddleFillPattern--) | Gantt çubuğunun dolgu desenini alır. |
| [getMiddleShape()](#getMiddleShape--) | Çubuğun orta şekli alır. |
| [getMiddleShapeColor()](#getMiddleShapeColor--) | Orta şeklin rengini alır. |
| [getName()](#getName--) | Stil adını alır. |
| [getParentStyle()](#getParentStyle--) | Özel görev‑spesifik stil için üst (veya ortak) stili alır. |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | Görevin çubuğunun sağ tarafında görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. |
| [getRightField()](#getRightField--) | Çubuğun sağ tarafında görüntülenecek veriyi alır. |
| [getRow()](#getRow--) | Satır numarasını alır. |
| [getShowForCategories()](#getShowForCategories--) | Stilin uygulandığı görev kategorilerini alır. |
| [getShowForTaskUid()](#getShowForTaskUid--) | Stilin uygulandığı görevin benzersiz kimliğini alır. |
| [getStartShape()](#getStartShape--) | Çubuğun başlangıç şekli alır. |
| [getStartShapeColor()](#getStartShapeColor--) | Başlangıç şeklinin rengini alır. |
| [getStartShapeType()](#getStartShapeType--) | Başlangıç şeklinin tipini alır. |
| [getTo()](#getTo--) | Gantt çubuğunun bitiş noktası konumunu alır. |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | Görevin çubuğunun üst kısmında görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. |
| [getTopField()](#getTopField--) | Çubuğun üst kısmında görüntülenecek veriyi alır. |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Görevin çubuğunun alt kısmında görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü ayarlar. |
| [setBottomField(int value)](#setBottomField-int-) | Çubuğun alt kısmında görüntülenecek veriyi ayarlar. |
| [setEndShape(int value)](#setEndShape-int-) | Çubuğun bitiş şekli ayarlar. |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | Bitiş şeklinin rengini ayarlar. |
| [setEndShapeType(int value)](#setEndShapeType-int-) | Bitiş şeklinin tipini ayarlar. |
| [setFrom(int value)](#setFrom-int-) | Gantt çubuğunun başlangıç noktası konumunu ayarlar. |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Görevin çubuğunun içinde görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü ayarlar. |
| [setInsideField(int value)](#setInsideField-int-) | Çubuğun içinde görüntülenecek veriyi ayarlar. |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Görevin çubuğunun sol tarafında görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü ayarlar. |
| [setLeftField(int value)](#setLeftField-int-) | Çubuğun sol tarafında görüntülenecek veriyi ayarlar. |
| [setMiddleFillPattern(int value)](#setMiddleFillPattern-int-) | Gantt çubuğunun doldurma desenini ayarlar. |
| [setMiddleShape(int value)](#setMiddleShape-int-) | Çubuğun orta şekli ayarlanır. |
| [setMiddleShapeColor(Color value)](#setMiddleShapeColor-java.awt.Color-) | Orta şeklin rengi ayarlanır. |
| [setName(String value)](#setName-java.lang.String-) | Stilin adı ayarlanır. |
| [setParentStyle(GanttBarStyle value)](#setParentStyle-com.aspose.tasks.GanttBarStyle-) | Özel görev‑özel stili için üst (veya ortak) stil ayarlanır. |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Görevin çubuğunun sağında görüntülenecek metni almak için kullanıcı tanımlı dönüştürücü ayarlanır. |
| [setRightField(int value)](#setRightField-int-) | Çubuğun sağında görüntülenecek veri ayarlanır. |
| [setRow(int value)](#setRow-int-) | Satır numarası ayarlanır. |
| [setShowForCategories(List&lt;Integer&gt; value)](#setShowForCategories-java.util.List-java.lang.Integer--) | Stilin uygulanacağı görev kategorileri ayarlanır. |
| [setShowForTaskUid(Integer value)](#setShowForTaskUid-java.lang.Integer-) | Stilin uygulanacağı görevin benzersiz kimliği ayarlanır. |
| [setStartShape(int value)](#setStartShape-int-) | Çubuğun başlangıç şekli ayarlanır. |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | Başlangıç şeklinin rengi ayarlanır. |
| [setStartShapeType(int value)](#setStartShapeType-int-) | Başlangıç şeklinin türü ayarlanır. |
| [setTo(int value)](#setTo-int-) | Gantt çubuğunun bitiş noktası konumu ayarlanır. |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Görevin çubuğunun üstünde görüntülenecek metni almak için kullanıcı tanımlı dönüştürücü ayarlanır. |
| [setTopField(int value)](#setTopField-int-) | Çubuğun üstünde görüntülenecek veri ayarlanır. |
### GanttBarStyle() {#GanttBarStyle--}
```
public GanttBarStyle()
```


[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) sınıfının yeni bir örneğini başlatır.

### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


Görevin çubuğunun altında görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


Çubuğun altında görüntülenecek veriyi alır. [Field](../../com.aspose.tasks/field).

**Returns:**
int - çubuğun altında görüntülenecek veri.
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


Çubuğun son şekli alır.

**Returns:**
int - çubuğun bitiş şekli.
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


Son şeklin rengini alır.

**Returns:**
java.awt.Color - bitiş şeklinin rengi.
### getEndShapeType() {#getEndShapeType--}
```
public final int getEndShapeType()
```


Bitiş şeklinin türünü alır. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Returns:**
int - bitiş şeklinin türü.
### getFrom() {#getFrom--}
```
public final int getFrom()
```


Gantt çubuğunun başlangıç noktası konumunu alır. [Field](../../com.aspose.tasks/field).

**Returns:**
int - gantt çubuğunun başlangıç noktası konumu.
### getInsideBarTextConverter() {#getInsideBarTextConverter--}
```
public final TaskBarTextConverter getInsideBarTextConverter()
```


Görev çubuğunun içinde işlenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. `InsideField`([getInsideField()](../../com.aspose/tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose/tasks/ganttbarstyle\#setInsideField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


Çubuğun içinde görüntülenecek veriyi alır. [Field](../../com.aspose/tasks/field).

**Returns:**
int - çubuğun içinde görüntülenecek veri.
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


Görev çubuğunun solunda işlenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. `LeftField`([getLeftField()](../../com.aspose/tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose/tasks/ganttbarstyle\#setLeftField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


Çubuğun solunda görüntülenecek veriyi alır. [Field](../../com.aspose/tasks/field).

**Returns:**
int - çubuğun solunda görüntülenecek veri.
### getMiddleFillPattern() {#getMiddleFillPattern--}
```
public final int getMiddleFillPattern()
```


Gantt çubuğunun dolgu desenini alır.

**Returns:**
int - gantt çubuğunun dolgu deseni.
### getMiddleShape() {#getMiddleShape--}
```
public final int getMiddleShape()
```


Çubuğun orta şekli alır.

**Returns:**
int - çubuğun orta şekli.
### getMiddleShapeColor() {#getMiddleShapeColor--}
```
public final Color getMiddleShapeColor()
```


Orta şeklin rengini alır.

**Returns:**
java.awt.Color - orta şeklin rengi.
### getName() {#getName--}
```
public final String getName()
```


Stil adını alır.

**Returns:**
java.lang.String - stilin adı.
### getParentStyle() {#getParentStyle--}
```
public final GanttBarStyle getParentStyle()
```


Özel görev‑spesifik stil için üst (veya ortak) stili alır.

--------------------

Görev, farklı üst stillere sahip birden fazla özel stile sahip olabilir. Örneğin, "Critical" üst stiline sahip bir özel stil ve "Normal" üst stiline sahip başka bir stil düşünün. Kısaca, görev kritikse, ilk stil uygulanır. Görev kritik olmadığında, ikinci stil uygulanır (bu mantık Microsoft Project Professional'dan miras alınmıştır).

**Returns:**
[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) - parent (or common) style for custom task-specific style.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


Görev çubuğunun sağında işlenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. `RightField`([getRightField()](../../com.aspose/tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose/tasks/ganttbarstyle\#setRightField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


Çubuğun sağında görüntülenecek veriyi alır. [Field](../../com.aspose/tasks/field).

**Returns:**
int - çubuğun sağında görüntülenecek veri.
### getRow() {#getRow--}
```
public final int getRow()
```


Satır numarasını alır.

--------------------

1 ile 4 arasında olabilir (1 varsayılan değerdir).

**Returns:**
int - bir satır numarası.
### getShowForCategories() {#getShowForCategories--}
```
public final List<Integer> getShowForCategories()
```


Stilin uygulandığı görev kategorilerini alır. Gantt şemasındaki çubukların üst (veya ortak) stilleri için geçerlidir (`GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose/tasks/ganttchartview\#getBarStyles--))).

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - stilin uygulandığı görev kategorileri.
### getShowForTaskUid() {#getShowForTaskUid--}
```
public final Integer getShowForTaskUid()
```


Stilin uygulandığı görevin benzersiz kimliğini alır. Gantt şemasındaki çubukların göreve özgü stilleri için geçerlidir (`GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose/tasks/ganttchartview\#getCustomBarStyles--))).

**Returns:**
java.lang.Integer - stilin uygulandığı görevin benzersiz kimliği.
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


Çubuğun başlangıç şekli alır.

**Returns:**
int - çubuğun başlangıç şekli.
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


Başlangıç şeklinin rengini alır.

**Returns:**
java.awt.Color - başlangıç şeklinin rengi.
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


Başlangıç şeklinin tipini alır.

**Returns:**
int - başlangıç şeklinin türü.
### getTo() {#getTo--}
```
public final int getTo()
```


Gantt çubuğunun bitiş noktası konumunu alır.

**Returns:**
int - gantt çubuğunun bitiş noktası konumu.
### getTopBarTextConverter() {#getTopBarTextConverter--}
```
public final TaskBarTextConverter getTopBarTextConverter()
```


Görev çubuğunun üstünde işlenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır. `TopField`([getTopField()](../../com.aspose/tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose/tasks/ganttbarstyle\#setTopField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


Çubuğun üst kısmında görüntülenecek veriyi alır.

**Returns:**
int - çubuğun üst kısmında görüntülenecek veri.
### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


Görev çubuğunun alt kısmında işlenecek metni almak için kullanıcı tanımlı dönüştürücüyü ayarlar. `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Görev çubuğunun alt kısmında işlenecek metni almak için kullanıcı tanımlı dönüştürücü. |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


Çubuğun alt kısmında görüntülenecek veriyi ayarlar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Çubuğun alt kısmında görüntülenecek veri. |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


Çubuğun bitiş şekli ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | çubuğun uç şekli. |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


Bitiş şeklinin rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | uç şeklinin rengi. |

### setEndShapeType(int value) {#setEndShapeType-int-}
```
public final void setEndShapeType(int value)
```


Uç şeklin tipini ayarlar. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | uç şeklin tipi. |

### setFrom(int value) {#setFrom-int-}
```
public final void setFrom(int value)
```


Gantt çubuğunun başlangıç noktası konumunu ayarlar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Gantt çubuğunun başlangıç noktası konumu. |

### setInsideBarTextConverter(TaskBarTextConverter value) {#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setInsideBarTextConverter(TaskBarTextConverter value)
```


Görev çubuğunun içinde işlenecek metni almak için kullanıcı tanımlı dönüştürücüyü ayarlar. `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Görev çubuğunun içinde işlenecek metni almak için kullanıcı tanımlı dönüştürücü. |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


Çubuğun içinde görüntülenecek veriyi ayarlar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Çubuğun içinde görüntülenecek veri. |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


Görev çubuğunun sol tarafında işlenecek metni almak için kullanıcı tanımlı dönüştürücüyü ayarlar. `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Görev çubuğunun sol tarafında işlenecek metni almak için kullanıcı tanımlı dönüştürücü. |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


Çubuğun sol tarafında görüntülenecek veriyi ayarlar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Çubuğun sol tarafında görüntülenecek veri. |

### setMiddleFillPattern(int value) {#setMiddleFillPattern-int-}
```
public final void setMiddleFillPattern(int value)
```


Gantt çubuğunun doldurma desenini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | gantt çubuğunun dolgu deseni. |

### setMiddleShape(int value) {#setMiddleShape-int-}
```
public final void setMiddleShape(int value)
```


Çubuğun orta şekli ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | çubuğun orta şekli. |

### setMiddleShapeColor(Color value) {#setMiddleShapeColor-java.awt.Color-}
```
public final void setMiddleShapeColor(Color value)
```


Orta şeklin rengi ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | orta şeklin rengi. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Stilin adı ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | stilin adı. |

### setParentStyle(GanttBarStyle value) {#setParentStyle-com.aspose.tasks.GanttBarStyle-}
```
public final void setParentStyle(GanttBarStyle value)
```


Özel görev‑özel stili için üst (veya ortak) stil ayarlanır.

--------------------

Görev, farklı üst stillere sahip birden fazla özel stile sahip olabilir. Örneğin, "Critical" üst stiline sahip bir özel stil ve "Normal" üst stiline sahip başka bir stil düşünün. Kısaca, görev kritikse, ilk stil uygulanır. Görev kritik olmadığında, ikinci stil uygulanır (bu mantık Microsoft Project Professional'dan miras alınmıştır).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) | özel görev‑spesifik stil için üst (veya ortak) stil. |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


Görev çubuğunun sağ tarafında işlenecek metni almak için kullanıcı tanımlı dönüştürücüyü ayarlar. `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | görev çubuğunun sağında render edilecek metni almak için kullanıcı tanımlı dönüştürücü. |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


Çubuğun sağında görüntülenecek verileri ayarlar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | çubuğun sağında görüntülenecek veri. |

### setRow(int value) {#setRow-int-}
```
public final void setRow(int value)
```


Satır numarası ayarlanır.

--------------------

1 ile 4 arasında olabilir (1 varsayılan değerdir).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir satır numarası. |

### setShowForCategories(List&lt;Integer&gt; value) {#setShowForCategories-java.util.List-java.lang.Integer--}
```
public final void setShowForCategories(List<Integer> value)
```


Stilinin uygulandığı görev kategorilerini ayarlar. Gantt şemasındaki çubukların üst (veya ortak) stillerine uygulanabilir (bkz. `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.List&lt;java.lang.Integer&gt; | stilin uygulandığı görev kategorileri. |

### setShowForTaskUid(Integer value) {#setShowForTaskUid-java.lang.Integer-}
```
public final void setShowForTaskUid(Integer value)
```


Stilin uygulandığı bir görevin Unique Id'sini ayarlar. Gantt şemasındaki çubukların görev‑özelliği stillerine uygulanabilir (bkz. `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Integer | Stilin uygulandığı bir görevin Unique Id'si. |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


Çubuğun başlangıç şekli ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | çubuğun başlangıç şekli. |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


Başlangıç şeklinin rengi ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | başlangıç şeklinin rengi. |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


Başlangıç şeklinin türü ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | başlangıç şeklinin tipi. |

### setTo(int value) {#setTo-int-}
```
public final void setTo(int value)
```


Gantt çubuğunun bitiş noktası konumu ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | gantt çubuğunun bitiş noktası konumu. |

### setTopBarTextConverter(TaskBarTextConverter value) {#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setTopBarTextConverter(TaskBarTextConverter value)
```


Görev çubuğunun üstünde render edilecek metni almak için kullanıcı tanımlı dönüştürücüyü ayarlar. `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)) özelliğinin değerini geçersiz kılar.

--------------------

MPP formatına kaydedilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | görev çubuğunun üstünde render edilecek metni almak için kullanıcı tanımlı dönüştürücü. |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


Çubuğun üstünde görüntülenecek veri ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | çubuğun üstünde görüntülenecek veri. |

