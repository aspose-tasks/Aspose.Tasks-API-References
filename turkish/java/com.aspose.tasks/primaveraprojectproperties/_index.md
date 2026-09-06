---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Primavera dosyaları XER veya P6XML'den okunan bir proje için Primavera'ya özgü özellikleri temsil eder."
type: docs
weight: 205
url: /tr/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Primavera dosyalarından (XER veya P6XML) okunan bir proje için Primavera'ya özgü özellikleri temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Geçerli projenin temel projeler dizisini alır. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Kritik aktiviteleri tanımlama yöntemini alır: En Uzun Yol ya da Toplam Yüzerlik yaklaşımı. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Toplam Yüzerlik yöntemi kullanıldığında kritik aktiviteleri tanımlamak için kullanılan eşik değerini alır. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Geçerli temel projenin kimliğini alır. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Projeler arasındaki aktivite ilişkilerini yok sayıp saymayacağını tanımlayan bir bayrağı alır. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Projeyi zamanlarken aktivitelerin kritik olarak işaretlenip işaretlenmeyeceğini tanımlayan bir bayrağı alır. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Primavera projelerinde İlişki Gecikmesini zamanlamak için kullanılacak takvimi tanımlayan bir seçeneği alır. |
| [getShortName()](#getShortName--) | Projenin kısa adını (Proje Kimliği) alır. |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Aktivite bitiş tarihlerinin beklenen bitiş tarihleri olarak zamanlanıp zamanlanmayacağını tanımlayan bir bayrağı alır. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Geçerli projenin temel projeler dizisini alır. Dışa aktarılmış temelleri içeren Primavera XML dosyalarından okunan projeler için geçerlidir.

**Returns:**
com.aspose.tasks.Project[] - geçerli projenin temel projeler dizisi.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Kritik aktiviteleri tanımlama yöntemini alır: En Uzun Yol ya da Toplam Yüzerlik yaklaşımı.

**Returns:**
int - kritik aktiviteleri tanımlama yöntemi: En Uzun Yol ya da Toplam Yüzerlik yaklaşımı.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Toplam Yüzerlik yöntemi kullanıldığında kritik aktiviteleri tanımlamak için kullanılan eşik değerini alır.

**Returns:**
java.lang.Double - Toplam Yüzerlik yöntemi kullanıldığında kritik aktiviteleri tanımlamak için kullanılan eşik değeri.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Geçerli temel projenin kimliğini alır. Dışa aktarılmış temelleri içeren Primavera XML dosyalarından okunan projeler için geçerlidir.

**Returns:**
int - Mevcut temel projenin kimliği.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Projeler arasındaki aktivite ilişkilerini yok sayıp saymayacağını tanımlayan bir bayrağı alır.

**Returns:**
boolean - projeler arasındaki aktivite ilişkilerini yok sayıp saymayacağını tanımlayan bir bayrak.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Projeyi zamanlarken aktivitelerin kritik olarak işaretlenip işaretlenmeyeceğini tanımlayan bir bayrağı alır.

**Returns:**
boolean - projenin zamanlanması sırasında aktivitelerin kritik olarak işaretlenip işaretlenmeyeceğini tanımlayan bir bayrak.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Primavera projelerinde İlişki Gecikmesini zamanlamak için kullanılacak takvimi tanımlayan bir seçeneği alır.

**Returns:**
int - Primavera projelerinde İlişki Gecikmesi zamanlaması için hangi takvimin kullanılacağını tanımlayan bir seçenek.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Projenin kısa adını (Proje Kimliği) alır.

**Returns:**
java.lang.String - projenin kısa adı (Proje Kimliği).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Aktivite bitiş tarihlerinin beklenen bitiş tarihleri olarak zamanlanıp zamanlanmayacağını tanımlayan bir bayrağı alır.

**Returns:**
boolean - aktivite bitiş tarihlerinin beklenen bitiş tarihleri olarak zamanlanıp zamanlanmayacağını tanımlayan bir bayrak.
