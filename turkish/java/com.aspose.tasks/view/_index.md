---
title: "View"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Project içinde bir görünümü temsil eder."
type: docs
weight: 342
url: /tr/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Project içinde bir görünümü temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [View()](#View--) | Yeni bir [View](../../com.aspose.tasks/view) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Mevcut örneği aynı türdeki başka bir nesneyle karşılaştırır ve mevcut örneğin diğer nesneye göre sıralama düzeninde önce mi, sonra mı yoksa aynı konumda mı olduğunu gösteren bir tamsayı döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Yeni bir [View](../../com.aspose.tasks/view) sınıfı örneği oluşturur. |
| [getFilter()](#getFilter--) | Tek bir görünümde kullanılan bir filtreyi alır. |
| [getGroup()](#getGroup--) | Tek bir görünümün bir grubunu alır. |
| [getHighlightFilter()](#getHighlightFilter--) | Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamadığını gösteren bir değeri alır. |
| [getName()](#getName--) | Bir View nesnesinin adını alır. |
| [getPageInfo()](#getPageInfo--) | `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\\#getPageInfo--)) sınıfının bir örneğini alır. |
| [getParentProject()](#getParentProject--) | View nesnesinin üst nesnesini alır. |
| [getScreen()](#getScreen--) | Tek bir görünüm için ekran tipini alır. |
| [getShowInMenu()](#getShowInMenu--) | Microsoft Project'in Tek Görünüm adını View veya Diğer Görünümler açılır listelerinde Ribbon'da gösterip göstermediğini belirten bir değeri alır. |
| [getTable()](#getTable--) | Tek bir görünümün tablosunu alır. |
| [getType()](#getType--) | Tek görünümdeki öğenin türünü alır, örneğin görevler veya kaynaklar. |
| [getUid()](#getUid--) | Bir görünümün benzersiz tanımlayıcısını alır. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Görünümdeki [OleObject](../../com.aspose.tasks/oleobject) konumunu ve görünümünü temsil eden nesneler koleksiyonunu alır. |
| [hashCode()](#hashCode--) | [Resource](../../com.aspose.tasks/resource) sınıfının örneği için bir hash kod değeri döndürür. |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değeri döndürür. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını belirten bir değeri döndürür. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değeri döndürür. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değeri döndürür. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını belirten bir değeri döndürür. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Tek bir görünümde kullanılan bir filtre ayarlar. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Tek görünümün bir grubunu ayarlar. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamadığını gösteren bir değeri ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Bir View nesnesinin adını ayarlar. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Microsoft Project'in Tek Görünüm adını Ribbon'daki View veya Other Views açılır listelerinde gösterip göstermediğini belirten bir değeri ayarlar. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Tek görünümün bir tablosunu ayarlar. |
### View() {#View--}
```
public View()
```


Yeni bir [View](../../com.aspose.tasks/view) sınıfı örneği başlatır.

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Mevcut örneği aynı türdeki başka bir nesneyle karşılaştırır ve mevcut örneğin diğer nesneye göre sıralama düzeninde önce mi, sonra mı yoksa aynı konumda mı olduğunu gösteren bir tamsayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | bu örneğin karşılaştırılacağı belirtilen View nesnesi. |

**Returns:**
int - Karşılaştırılan nesnelerin göreli sırasını gösteren 32 bit işaretli bir tam sayı. Dönüş değeri şu anlamlara gelir: Değer Anlamı Sıfırdan küçük Bu örnek sıralama düzeninde `other` öğesinden önce gelir. Sıfır Bu örnek `other` öğesiyle aynı konumda bulunur. Sıfırdan büyük Bu örnek sıralama düzeninde `other` öğesinden sonra gelir.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnek ile karşılaştırılacak nesne. |

**Returns:**
boolean - **True** ise belirtilen nesne bu örnekle aynı Uid değerine sahip bir View'dir; aksi takdirde **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Yeni bir [View](../../com.aspose.tasks/view) sınıfı örneği oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| viewScreen | int | Görünümün görüntülenebileceği ekran türü. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Tek bir görünümde kullanılan bir filtreyi alır.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Tek bir görünümün bir grubunu alır.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamadığını gösteren bir değeri alır.

**Returns:**
boolean - Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamadığını gösteren bir değer.
### getName() {#getName--}
```
public final String getName()
```


Bir View nesnesinin adını alır.

**Returns:**
java.lang.String - bir View nesnesinin adı.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


`PageInfo` sınıfının bir örneğini alır ([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). mpp dosya formatında bulunan sayfa ayarı verilerini temsil eder.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


View nesnesinin üst öğesini alır. Salt okunur [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Tek görünüm için ekran türünü alır. Salt okunur [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - tek görünüm için ekran türü.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Microsoft Project'in Tek Görünüm adını View veya Diğer Görünümler açılır listelerinde Ribbon'da gösterip göstermediğini belirten bir değeri alır.

**Returns:**
boolean - Microsoft Project'in Tek Görünüm adını Ribbon'daki View veya Other Views açılır listelerinde gösterip göstermediğini belirten bir değer.
### getTable() {#getTable--}
```
public final Table getTable()
```


Tek bir görünümün tablosunu alır.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Tek görünümdeki öğenin türünü alır, örneğin görevler veya kaynaklar. Salt okunur [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - tek görünümdeki öğenin türü, örneğin görevler veya kaynaklar.
### getUid() {#getUid--}
```
public final int getUid()
```


Bir görünümün benzersiz tanımlayıcısını alır.

**Returns:**
int - bir görünümün benzersiz tanımlayıcısı.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Görünümdeki [OleObject](../../com.aspose.tasks/oleobject) konumunu ve görünümünü temsil eden nesneler koleksiyonunu alır.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - Görünümdeki [OleObject](../../com.aspose.tasks/oleobject) konumunu ve görünümünü temsil eden nesneler koleksiyonu.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[Resource](../../com.aspose.tasks/resource) sınıfının örneği için bir hash kod değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | İlk görünüm. |
| b | [View](../../com.aspose.tasks/view) | İkinci görünüm. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değer
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | İlk görünüm. |
| b | [View](../../com.aspose.tasks/view) | İkinci görünüm. |

**Returns:**
boolean - bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değer
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | İlk görünüm. |
| b | [View](../../com.aspose.tasks/view) | İkinci görünüm. |

**Returns:**
boolean - bu örneğin belirtilen nesneden büyük ya da ona eşit olup olmadığını belirten bir değer
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | İlk görünüm. |
| b | [View](../../com.aspose.tasks/view) | İkinci görünüm. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değer
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | İlk filtre. |
| b | [View](../../com.aspose.tasks/view) | İkinci filtre. |

**Returns:**
boolean - bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değer
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | İlk görünüm. |
| b | [View](../../com.aspose.tasks/view) | İkinci görünüm. |

**Returns:**
boolean - bu örneğin belirtilen nesneden küçük ya da ona eşit olup olmadığını belirten bir değer
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Tek bir görünümde kullanılan bir filtre ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | Tek bir görünümde kullanılan bir filtre. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Tek görünümün bir grubunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | Tek görünümün bir grubu. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamadığını gösteren bir değer. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Bir View nesnesinin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Bir View nesnesinin adı. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Microsoft Project'in Tek Görünüm adını Ribbon'daki View veya Other Views açılır listelerinde gösterip göstermediğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Microsoft Project'in Tek Görünüm adını Şerit'teki Görünüm veya Diğer Görünümler açılır listelerinde gösterip göstermediğini belirten bir değer. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Tek görünümün bir tablosunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | Tek görünümün bir tablosu. |

