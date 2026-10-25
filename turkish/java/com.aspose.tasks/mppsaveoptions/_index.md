---
title: "MPPSaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje verilerini MPP'ye kaydederken ek seçenekler belirtmeye izin verir."
type: docs
weight: 149
url: /tr/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Proje verilerini MPP'ye kaydederken ek seçenekler belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Yeni bir [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getClearVba()](#getClearVba--) | Projeyi MPP formatında kaydederken mevcut VBA makro verilerini kaldırıp kaldırmayacağını gösteren bir değer alır. |
| [getProtectionPassword()](#getProtectionPassword--) | Oluşturulan MPP dosyasını korumak için kullanılan bir şifre alır. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | MPP'ye kaydederken geçersiz kaynak atamalarını kaldırıp kaldırmayacağını gösteren bir değer alır. |
| [getWriteFilters()](#getWriteFilters--) | Projeyi MPP formatına kaydederken filtre verilerini yazıp yazmayacağını gösteren bir değer alır. |
| [getWriteGroups()](#getWriteGroups--) | Bir projenin MPP formatında kaydedilirken grup verilerinin yazılıp yazılmayacağını gösteren bir değeri alır. |
| [getWriteVba()](#getWriteVba--) | MPP dosyasındaki mevcut VBA makro verilerinin güncellenip güncellenmeyeceğini gösteren bir değeri alır. |
| [getWriteViewData()](#getWriteViewData--) | Bir projenin MPP formatında kaydedilirken görünüm verilerinin yazılıp yazılmayacağını gösteren bir değeri alır. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Bir projenin MPP formatında kaydedilirken mevcut VBA makro verilerinin kaldırılıp kaldırılmayacağını gösteren bir değeri ayarlar. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Ortaya çıkan MPP dosyasını korumak için kullanılan bir şifreyi ayarlar. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | MPP'ye kaydedilirken geçersiz kaynak atamalarının kaldırılıp kaldırılmayacağını gösteren bir değeri ayarlar. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Bir projenin MPP formatında kaydedilirken filtre verilerinin yazılıp yazılmayacağını gösteren bir değeri ayarlar. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Bir projenin MPP formatında kaydedilirken grup verilerinin yazılıp yazılmayacağını gösteren bir değeri ayarlar. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | MPP dosyasındaki mevcut VBA makro verilerinin güncellenip güncellenmeyeceğini gösteren bir değeri ayarlar. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Bir projenin MPP formatında kaydedilirken görünüm verilerinin yazılıp yazılmayacağını gösteren bir değeri ayarlar. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Yeni bir [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) sınıfı örneği başlatır.

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Projeyi MPP formatında kaydederken mevcut VBA makro verilerini kaldırıp kaldırmayacağını gösteren bir değer alır.

**Returns:**
boolean - bir projenin MPP formatında kaydedilirken mevcut VBA makro verilerinin kaldırılıp kaldırılmayacağını gösteren bir değer.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Ortaya çıkan MPP dosyasını korumak için kullanılan bir şifreyi alır. Şu anda MS Project 2010 ve daha yeni formatlar için desteklenmektedir.

--------------------

Null değeri, proje dosyasının korunmadığını gösterir.

**Returns:**
java.lang.String - ortaya çıkan MPP dosyasını korumak için kullanılan bir şifre.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


MPP'ye kaydederken geçersiz kaynak atamalarını kaldırıp kaldırmayacağını gösteren bir değer alır.

--------------------

MS Project, her görev için boş bir kaynak ataması oluşturur. Kaydetme sırasında bunları kaldırmak için bu bayrağı true olarak ayarlayın.

**Returns:**
boolean - MPP'ye kaydedilirken geçersiz kaynak atamalarının kaldırılıp kaldırılmayacağını gösteren bir değer.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Projeyi MPP formatına kaydederken filtre verilerini yazıp yazmayacağını gösteren bir değer alır.

--------------------

Filtre verileri, Project.TaskFilters ve Project.ResourceFilters koleksiyonlarını içerir.

--------------------

Şu anda MSP 2010 ve daha yeni formatlar için desteklenmektedir.

**Returns:**
boolean - bir projenin MPP formatında kaydedilirken filtre verilerinin yazılıp yazılmayacağını gösteren bir değer.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Bir projenin MPP formatında kaydedilirken grup verilerinin yazılıp yazılmayacağını gösteren bir değeri alır.

--------------------

Grup verileri, Project.TaskGroups ve Project.ResourceGroups koleksiyonlarını içerir.

**Returns:**
boolean - bir projenin MPP formatında kaydedilirken grup verilerinin yazılıp yazılmayacağını gösteren bir değer.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


MPP dosyasındaki mevcut VBA makro verilerinin güncellenip güncellenmeyeceğini gösteren bir değeri alır. Şu anda VbaModule.SourceCode'un yazılması desteklenmektedir.

**Returns:**
boolean - MPP dosyasındaki mevcut VBA makro verilerinin güncellenip güncellenmeyeceğini gösteren bir değer.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Bir projenin MPP formatında kaydedilirken görünüm verilerinin yazılıp yazılmayacağını gösteren bir değeri alır.

--------------------

Görünüm verileri, Project.Views, Filters ve Tables koleksiyonlarını içerir.

**Returns:**
boolean - bir projenin MPP formatında kaydedilirken görünüm verilerinin yazılıp yazılmayacağını gösteren bir değer.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Bir projenin MPP formatında kaydedilirken mevcut VBA makro verilerinin kaldırılıp kaldırılmayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir proje MPP formatında kaydedilirken mevcut VBA makroları verisinin kaldırılıp kaldırılmayacağını gösteren bir değer. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Oluşturulan MPP dosyasını korumak için kullanılan bir parolayı ayarlar. Şu anda MS Project 2010 ve daha yeni formatlar için desteklenmektedir.

--------------------

Null değeri, proje dosyasının korunmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | oluşturulan MPP dosyasını korumak için kullanılan bir parola. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


MPP'ye kaydedilirken geçersiz kaynak atamalarının kaldırılıp kaldırılmayacağını gösteren bir değeri ayarlar.

--------------------

MS Project, her görev için boş bir kaynak ataması oluşturur. Kaydetme sırasında bunları kaldırmak için bu bayrağı true olarak ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | MPP'ye kaydedilirken geçersiz kaynak atamalarının kaldırılıp kaldırılmayacağını gösteren bir değer. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Bir projenin MPP formatında kaydedilirken filtre verilerinin yazılıp yazılmayacağını gösteren bir değeri ayarlar.

--------------------

Filtre verileri, Project.TaskFilters ve Project.ResourceFilters koleksiyonlarını içerir.

--------------------

Şu anda MSP 2010 ve daha yeni formatlar için desteklenmektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir proje MPP formatına kaydedilirken filtre verisinin yazılıp yazılmayacağını gösteren bir değer. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Bir projenin MPP formatında kaydedilirken grup verilerinin yazılıp yazılmayacağını gösteren bir değeri ayarlar.

--------------------

Grup verileri, Project.TaskGroups ve Project.ResourceGroups koleksiyonlarını içerir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir proje MPP formatına kaydedilirken grup verisinin yazılıp yazılmayacağını gösteren bir değer. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


MPP dosyasındaki mevcut VBA makroları verisinin güncellenip güncellenmeyeceğini gösteren bir değeri ayarlar. Şu anda VbaModule.SourceCode yazımı desteklenmektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | MPP dosyasındaki mevcut VBA makroları verisinin güncellenip güncellenmeyeceğini gösteren bir değer. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Bir projenin MPP formatında kaydedilirken görünüm verilerinin yazılıp yazılmayacağını gösteren bir değeri ayarlar.

--------------------

Görünüm verileri, Project.Views, Filters ve Tables koleksiyonlarını içerir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir proje MPP formatında kaydedilirken görünüm verisinin yazılıp yazılmayacağını gösteren bir değer. |

